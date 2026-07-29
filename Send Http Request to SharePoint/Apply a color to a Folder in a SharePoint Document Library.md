# Apply a Color to a Colder in SharePoint Document Library
> Use this template to add an alternative color to a folder within a SharePoint document library using the 'Send HTTP Request to SharePoint' action. You'll need to refer to the table of available colors to use within the action.

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
_api/foldercoloring/stampcolor(DecodedUrl='<YourFoldersFullPath>') 
```
Headers:
```
{
  "Accept": "application/json;odata=nometadata",
  "Content-Type": "application/json;odata=verbose"
}
```
Body:
```
{   
   "coloringInformation": {     
      "ColorHex":"<ColorFromChartBelow>"
   }
}
```
## Color Table
| Color | Color Hex |
|---|---|
| Yellow | Empty or 0 (Default) |
| Dark red | 1 |
| Dark orange | 2 |
| Dark green | 3 |
| Dark teal | 4 |
| Dark blue | 5 |
| Dark purple | 6 |
| Dark pink | 7 |
| Grey | 8 |
| Light red | 9 |
| Light orange | 10 |
| Light green | 11 |
| Light teal | 12 |
| Light blue | 13 |
| Light purple | 14 |
| Light pink | 15 |