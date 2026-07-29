# Add Content-Type to SharePoint Document Library
Use this template to add a Content-Type to a SharePoint document library using the 'Send HTTP Request to SharePoint' action.

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
_api/web/lists/getbyID('{YourTargetLibraryGUID}')/contenttypes/addAvailableContentType
```
Headers:
```
{
  "accept": "application/json;odata=verbose",
  "content-type": "application/json;odata=verbose"
}
```
Body:
```
{
  "contentTypeId": "{YourContentTypeID}"
}
```
