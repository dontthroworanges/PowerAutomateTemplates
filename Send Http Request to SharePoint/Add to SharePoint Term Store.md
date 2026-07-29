# Add Value to SharePoint Term Store
Use this template to push a value to the SharePoint Term Store. 
## Basic Version
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
_api/v2.1/termStore/groups('{termgroupID}')/sets('{termsetID}')/children
```
Body:
```
{
    "labels": [
        {
            "name": "{YouTermName}",
            "isDefault": true,
            "languageTag": "en-US"
        }
    ]
}
