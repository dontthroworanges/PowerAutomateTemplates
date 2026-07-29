# Remove All Special Characters from String
> This expression removes all special characters including spaces from a string. 

Action Used: 
```
Compose
```
Expression:
```
replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(replace(triggerBody()?['PPMProject_ProjectName'], '/', '-'), '!', ''), '@', ''), '#', ''), '$', ''), '%', ''), '^', ''), '&', ''), '*', ''), '(', ''), ')', ''), '+', ''), '=', ''), '{', ''), '}', ''), '[', ''), ']', ''), '|', ''), '\', ''), ':', ''), ';', ''), '"', ''), '''''', ''), '<', ''), '>', ''), ',', ''), '.', ''), '?', ''), '~', ''), '`', '')
```