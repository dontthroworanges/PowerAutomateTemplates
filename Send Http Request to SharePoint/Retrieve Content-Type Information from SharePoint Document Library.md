# Retrieve Content-Type Information from SharePoint Document Library
Use this template to retieve the information about a Content-Type within a SharePoint document library. The URI listed below shows the default 'Document' Content-Type as an example. 

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
_api/web/lists/getbyID('{YourLibraryGUID}')/ContentTypes?$filter=Name eq 'Document'
```