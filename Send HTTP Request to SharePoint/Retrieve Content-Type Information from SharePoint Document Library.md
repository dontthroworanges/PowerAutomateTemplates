# Retrieve Content-Type Information from SharePoint Document Library
> Use this template to retieve the information about a Content-Type within a SharePoint document library. The URI listed below shows the default 'Document' Content-Type as an example. You can then use a [Compose action](/Compose/Extract%20Content-Type%20ID%20from%20Output.md) to extract the StringId of the Content-Type for use in other actions. 

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
_api/web/lists/getbyID('<YourLibraryGUID>')/ContentTypes?$filter=Name eq 'Document'
```