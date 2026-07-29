# Publish a SharePoint Site Page
> Use this template to publish a SharePoint site page using the 'Send HTTP Request to SharePoint' action.

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
POST
```
URI:
```
_api/sitepages/pages(<PageItemID>)/publish
```
Headers:
```
{
  "Accept": "application/json;odata=verbose",
  "Content-Type": "application/json;odata=verbose"
}
```
Body:
```
{
  "__metadata": {
    "type": "SP.Publishing.SitePage"
  }
}
```