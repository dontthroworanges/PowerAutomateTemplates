# Extract Content-Type ID from Action Output
If you used the 'Retrieve Content-Type Information...' action, use this template to extract the Content-Type StringID for use in other actions. 

Action Used: 
```
Compose
```
Expression:
```
outputs('{YourRetieveContentTypeAction}')?['body']?['d']?['results']?[0]?['StringId']
```