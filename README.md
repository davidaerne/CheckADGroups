Retrieves Current User:  The program detects the currently logged-in Windows user using Environment.UserName and Environment.UserDomainName.

Interacts with Active Directory:  Uses PrincipalContext and UserPrincipal to fetch the user's group memberships.

Lists All Groups:  Displays all groups the user is currently a member of.

Checks Specific Groups: Compares the user's groups against a predefined list (groupsToCheck) and reports if the user belongs to each group.# CheckADGroups


Expected Output
When User Belongs to Groups
plaintext
Copy
Edit
Checking Active Directory group memberships...
Current User: DOMAIN\UserName

Groups the user is a member of:
- Domain Users
- IT Admins
- IT Scanners

Checking for specific groups:
[PASS] User is a member of 'Domain Admins'.
[FAIL] User is NOT a member of 'YourSecurityGroupName'.
[PASS] User is a member of 'IT Admins'.
[PASS] User is a member of 'IT Scanners'.
When User Does Not Exist in AD
plaintext
Copy
Edit
User not found in Active Directory.
