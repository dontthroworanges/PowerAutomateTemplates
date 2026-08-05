# Convert SharePoint Date-Time Column Format
> Use this compose action to convert the full time as returned by a SharePoint Date/Time column into different formats.

## Action Template

Action Used: 
```
Compose
```
For YYYY-MM-DD Use Inputs:
```
formatDateTime(<YourDynamicContentDate>, 'yyyy-MM-dd')
```
For DD-MM-YYYY Use Inputs:
```
formatDateTime(<YourDynamicContentDate>, 'dd-MM-yyyy')
```
