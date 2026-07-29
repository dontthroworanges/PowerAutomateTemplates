# If Get Items Action Returns No Results
> This condition can be used to stop a flow or trigger a subsequent action if your Get Items action returns nothing. 

## Action Template

Action Used: 
```
Condition
```
Value One:
```
length(outputs('Get_items')?['body/value'])
```
Operator:
```
is equal to
```
Value Two:
```
0
```