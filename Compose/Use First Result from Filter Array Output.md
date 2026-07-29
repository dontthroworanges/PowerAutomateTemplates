# Use First Result from Filter Array Output
> This expression can be handy if you are only expecting one item to be returned from a filter array action. Example could be a project number, email address, etc. 

## Action Template

Action Used: 
```
Compose
```
Expression:
```
first(body('Filter_array'))?['NameOfColumnToReturn']
```