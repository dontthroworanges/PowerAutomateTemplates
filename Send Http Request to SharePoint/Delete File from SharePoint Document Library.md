# Delete a file from a SharePoint Document Library
Use this template to delete a file from a SharePoint document library view using the 'Send HTTP Request to SharePoint' action.

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
_api/web/lists/getbyID('{YourDocumentLibraryGUID}')/items({YourItemIDToDelete})
```
Headers:
```
{
  "X-HTTP-Method": "DELETE",
  "IF-MATCH": "*"
}
```
