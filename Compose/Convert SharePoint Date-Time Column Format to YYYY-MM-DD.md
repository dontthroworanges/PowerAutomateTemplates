# Convert SharePoint Date-Time Column Format
> Use these compose action inputs to convert the full time as returned by a SharePoint Date/Time column into different formats.

## Action Template

Action Used: 
```
Compose
```
For YYYY-MM-DD Use Input:
```
formatDateTime(<YourDynamicContentDate>, 'yyyy-MM-dd')
```
For DD-MM-YYYY Use Input:
```
formatDateTime(<YourDynamicContentDate>, 'dd-MM-yyyy')
```
For "Day, Month DD, YYYY" Use Input:
```
formatDateTime(<YourDynamicContentDate>, 'dddd, MMMM dd, yyyy')
```
For "Mon DD, YYYY" Use Input:
```
formatDateTime(<YourDynamicContentDate>, 'MMM dd, yyyy')
```
## Common format specifiers cheat sheet
| Specifier | Meaning | Example |
|-----------|---------|---------|
| yyyy | 4-digit year | 2026 |
| MM | 2-digit month | 08 |
| MMM | Short month name | Aug |
| MMMM | Full month name | August |
| dd | 2-digit day | 06 |
| ddd | Short day name | Thu |
| dddd | Full day name | Thursday |
| HH | 24-hour hour | 14 |
| hh | 12-hour hour | 02 |
| mm | Minutes | 30 |
| ss | Seconds | 00 |
| tt | AM/PM | PM |
