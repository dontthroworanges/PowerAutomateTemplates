# Filter Query on Managed Metadata Column
> When using the Get Items (SharePoint) action, you aren't able to do a filter query on the column name when you are targetting a Managed Metadata column. This method isn't perfect but it's a good starting point. 

> [!NOTE]
> This method really only works if the column you are filtering on has unique values. You can still do a Filter Array to further refine your results. Just FYI. 

## Action Template

Action Used: 
```
Get Items
```
Filter Query
```
TaxCatchAll/Term eq '<ValueToFilterOn>'
```