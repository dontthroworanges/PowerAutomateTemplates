# Rename a Site Page
> Use this template to rename a SharePoint site page view using the 'Send HTTP Request to SharePoint' action. This action can be useful if you are creating shortened IDs for the page's url, but would like to then update the name to something understandable. Title is the name of the page that visitors will see at the top of the page. FileLeafRef is the internal page name which is what is used in the URL. 

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
_api/web/lists/getbyID('<YourSitePageLibraryGUID>')/items(<YourPageID>)
```
Headers:
```
{
  "content-type": "application/json;odata=verbose",
  "IF-MATCH": "*",
  "X-HTTP-METHOD": "PATCH"
}
```
Body:
```
{'__metadata':
{'type':'SP.Data.SitePagesItem'},
'Title':'<NewTitleOfPage>',
'FileLeafRef':'<NewInternalPageName>'
}
```