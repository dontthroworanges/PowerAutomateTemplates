# Get GUID of SharePoint Document Library
> Use this template to retrieve the GUID of a SharePoint document library using the 'Send HTTP Request to SharePoint' action.

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
_api/web/lists/getbytitle('<LibraryTitle>')
```
Headers:
```
{
  "Accept": "application/json;odata=verbose"
}
```

