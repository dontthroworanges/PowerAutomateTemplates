# Rename a SharePoint Document Library
> Use this template to rename a SharePoint document library using the 'Send HTTP Request to SharePoint' action.

> [!NOTE]
> This does not alter the URL of the library. It only updates the Display Name. 

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
_api/web/lists/getbyID('<YourDocumentLibraryGUID>')
```
Headers:
```
{
  "accept": "application/json;odata=verbose",
  "content-type": "application/json;odata=verbose",
  "X-HTTP-Method": "MERGE",
  "IF-MATCH": "*"
}
```
Body:
```
 {
  "__metadata": {
    "type": "SP.List"
  },
  "Title": "<NewDocumentLibraryName>"
}
```
