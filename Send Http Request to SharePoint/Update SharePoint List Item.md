# Update SharePoint List Item
> Use this action to update one or more fields in a SharePoint list. Using the 'Send HTTP Request to SharePoint' method avoids having potential blank values inserted into columns which do not need to be updated. By including 'bNewDocumentUpdate": false' in the body, the version number of the item will not be incremented. 

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
_api/web/lists/getbyID('<YourSharePointListID>')/items(<YourListItemID>)/ValidateUpdateListItem
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
  "formValues": [
    {
      "FieldName": "<InternalColumnName>",
      "FieldValue": "<ValueToInsertIntoColumn>"
    }
  ],
  "bNewDocumentUpdate": false
}
```
