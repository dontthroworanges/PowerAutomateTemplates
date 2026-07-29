# Get File Count from Get Files (Properties Only) Action
Returns the count of files found by the Get Files (Properties Only) action.

Action Used: 
```
Compose
```
Expression:
```
length(outputs('Get_files_(properties_only)')?['body/value'])
```