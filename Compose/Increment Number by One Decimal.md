# Create Random Seven Digit Number
> This expression takes a number field, adds 0.1 to it, rounds to one decimal place, and returns the result as a float. This is useful if you are creating child objects to it's parent which may have a set number. Example: Project 215 becomes Project 215.1 and so forth. 
## Action Template

Action Used: 
```
Compose
```
Expression:
```
float(formatNumber(add(float(<InputyourNumber>), 0.1), '0.0'))
```
