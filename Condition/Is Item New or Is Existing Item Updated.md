# Is Item New? Or Did It Previously Exist?
> This condition will allow you to create a single flow that can handle both new items and existing items that have been updated. 

## Action Template

Action Used: 
```
Condition
```
Value One:
```
triggerOutputs()?['body/{VersionNumber}']
```
Operator:
```
is equal to
```
Value Two:
```
1.0
```