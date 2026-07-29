# Extract Content-Type ID from Action Output
If you used the ['Retrieve Content-Type Information...'](https://github.com/dontthroworanges/PowerAutomateTemplates/blob/main/Send%20Http%20Request%20to%20SharePoint/Retrieve%20Content-Type%20Information%20from%20SharePoint%20Document%20Library.md) action, use this template to extract the Content-Type StringID for use in other actions. 

Action Used: 
```
Compose
```
Expression:
```
outputs('{YourRetieveContentTypeAction}')?['body']?['d']?['results']?[0]?['StringId']
```