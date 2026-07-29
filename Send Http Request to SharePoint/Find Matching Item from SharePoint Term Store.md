# Find Matching Item from SharePoint Term Store
> Use this template to retrieve a matching item from the SharePoint Term Store. 

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
GET
```
URI:
```
_api/v2.1/termStore/sets/<setId>/terms?$filter=labels/any(l:l/name eq '<YourMatchingValue>')
```