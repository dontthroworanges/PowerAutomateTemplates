# Delete a Content-Type from a SharePoint Document Library
> Use this template to delete a Content-Type from a SharePoint document library using the 'Send HTTP Request to SharePoint' action. You need to have the Content-Type's StringId in order to delete it from the library. See ['Retrieve Content-Type Information...'](https://github.com/dontthroworanges/PowerAutomateTemplates/blob/main/Send%20Http%20Request%20to%20SharePoint/Retrieve%20Content-Type%20Information%20from%20SharePoint%20Document%20Library.md) action for how to do this. 

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
_api/web/lists/getbytitle('{YourLibraryGUID}')/ContentTypes('{ContentTypeIDToBeDeleted}')/deleteObject() 
```

