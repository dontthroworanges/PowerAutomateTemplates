# Stop Infinite Loop Condition Using Service Account
> Use this method to stop a potential infinite loop condition when using the 'When an item is created or modified' action. You do not need to include the @domain

## Action Template

Trigger Condition:
```
@not(equals(triggerOutputs()?['body/Editor/DisplayName'],'<yourserviceaccountusername>'))
```
