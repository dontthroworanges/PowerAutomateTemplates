# Get GUID of SharePoint Document Library
> Use this template to retrieve the GUID of a SharePoint document library using the 'Send HTTP Request to SharePoint' action.

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
GET
```
URI:
```
_api/web/lists/getbytitle('{LibraryTitle}')
```
Headers:
```
{
  "Accept": "application/json;odata=verbose"
}
```

