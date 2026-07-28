# Add Value to SharePoint Term Store
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
            "name": "{StringToInsert}",
            "isDefault": true,
            "languageTag": "en-US"
        }
    ]
}
