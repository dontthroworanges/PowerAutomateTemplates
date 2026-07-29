# Extract List Item Entity Type Full Name from Output
> If you used the ['Get List Item Entity Type Full Name'](/Send%20HTTP%20Request%20to%20SharePoint/Get%20List%20Item%20Entity%20Type%20Full%20Name.md) action, use this template to extract the actual name for use in other actions. 

## Action Template

Action Used: 
```
Compose
```
Expression:
```
body('Send_an_HTTP_request_to_SharePoint')?['d']?['ListItemEntityTypeFullName']
```