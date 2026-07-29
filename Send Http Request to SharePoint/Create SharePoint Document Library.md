# Create a SharePoint Document Library
> Use this template to create a new SharePoint document library using the 'Send HTTP Request to SharePoint' action.

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
_api/web/lists
```
Headers:
```
{
  "accept": "application/json;odata=verbose",
  "content-type": "application/json;odata=verbose"
}
```
Body:
```
 {  
   '__metadata':{ 'type':'SP.List' },  
   'AllowContentTypes': true,   
   'BaseTemplate':101,   
   'ContentTypesEnabled':true,  
   'Description':"",   
   'Title': '<TitleOfNewDocLibrary>'
}
```
