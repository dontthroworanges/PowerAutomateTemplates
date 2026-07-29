# Rename a Folder or Document Set in a SharePoint Document Library
> Use this template to rename a folder or document set within a SharePoint Document Library using the 'Send HTTP Request to SharePoint' action.

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
_api/web/lists/getbyID('<YourLibraryGUID>')/items(<FolderDocSetID>)/ValidateUpdateListItem
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
      "FieldName": "FileLeafRef",
      "FieldValue": "<NewFolderName>"
    },
    {
      "FieldName": "Title",
      "FieldValue": "<NewFolderName>"
    }
  ],
  "bNewDocumentUpdate": false
}
```