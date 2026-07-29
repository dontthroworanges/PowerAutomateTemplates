# Add Term to SharePoint Term Store
> Use this template to push a term to the SharePoint Term Store using the 'Send HTTP Request to SharePoint' action.

## Action Template

Action Used: 
```
Send Http Request to SharePoint
```
Site Address:
```
Enter your site URL
```
Method:
```
POST
```
URI:
```
_api/v2.1/termStore/groups('<termgroupID>')/sets('<termsetID>')/children
```
### Term Only - No Synonyms or Additional Properties
Body:
```
{
    "labels": [
        {
            "name": "<TermName>",
            "isDefault": true,
            "languageTag": "en-US"
        }
    ]
}
```

### Term with Synonyms and Description
Body:
```
{
    "labels": [  
        {  
            "name": "<TermName>",  
            "isDefault": true,  
            "languageTag": "en-US"  
        },
        {  
            "name": "<Synonym1>",
            "isDefault": false,  
            "languageTag": "en-US"  
        },
        {  
            "name": "<Synonym2>",
            "isDefault": false,  
            "languageTag": "en-US"  
        }
    ],  
    "descriptions": [  
        {  
            "description": "<YourTermDescription>",  
            "languageTag": "en-US"  
        }  
    ]  
}
```
