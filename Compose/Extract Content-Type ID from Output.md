# Extract Content-Type ID from Action Output
If you used the ['Retrieve Content-Type Information...'](Send Http Request to SharePoint/Retrieve Content-Type Information from SharePoint Document Library.md) action, use this template to extract the Content-Type StringID for use in other actions. 

Action Used: 
```
Compose
```
Expression:
```
outputs('{YourRetieveContentTypeAction}')?['body']?['d']?['results']?[0]?['StringId']
```