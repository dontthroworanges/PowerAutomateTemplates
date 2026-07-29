# Add Column to a SharePoint Document Library View
> Use this template to add a column to a SharePoint document library view using the 'Send HTTP Request to SharePoint' action.

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
_api/web/lists/getbyID('{YourDocLibraryGUID}')/views/getByTitle('{ViewNameToAddColumnTo}')/viewfields/addviewfield('{InternalColumnNameToAddToView}')
```
Headers:
```
{
  "Accept": "application/json;odata=verbose",
  "Content-Type": "application/json;odata=verbose",
  "X-HTTP-Method": "MERGE",
  "IF-MATCH": "*"
}
```
