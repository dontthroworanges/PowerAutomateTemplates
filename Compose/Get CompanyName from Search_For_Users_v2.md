# Get CompanyName from Search_For_Users_v2
> Gets the Company Name of the first person found via a Search_for_users_v2 action 

## Action Template

Action Used: 
```
Compose
```
Expression:
```
first(body('Search_for_users_(V2)')?['value'])?['CompanyName']
```