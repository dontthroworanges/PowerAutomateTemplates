# Get List Item Entity Type Full Name
> Use this template to retrieve the ListItemEntityTypeFullName from a SharePoint Document Library. This is often needed in Send HTTP Request to SharePoint actions. 

## Action Template

Action Used: 
```
Send HTTP Request to SharePoint
```
Site Address:
```
<YourSiteURL>
```
Method:
```
GET
```
URI:
```
_api/web/lists/getbyID('<YourDocLibraryGUID>')?$select=ListItemEntityTypeFullName
```