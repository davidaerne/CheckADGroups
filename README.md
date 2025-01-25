Retrieves Current User:

The program detects the currently logged-in Windows user using Environment.UserName and Environment.UserDomainName.
Interacts with Active Directory:

Uses PrincipalContext and UserPrincipal to fetch the user's group memberships.
Lists All Groups:

Displays all groups the user is currently a member of.
Checks Specific Groups:

Compares the user's groups against a predefined list (groupsToCheck) and reports if the user belongs to each group.# CheckADGroups
