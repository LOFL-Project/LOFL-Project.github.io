---
Name: Get-ADUser
Description: Gets one or more Active Directory users
Updated: 2023-07-01
Toolsets:
  - RSAT
Commands:
  - Command: Get-ADUser -Filter {DoesNotRequirePreauth -eq $true}
    Description: List users based on filter
    Usecases:
      - Enumerate aseproastable users
    Function: Domain
    Comments:
      - 'PowerShell Module: `ActiveDirectory`'
    MitreAttack:
  - Command: 'Get-ADUser -Filter {ServicePrincipalName -ne "$null"} -Properties ServicePrincipalName'
    Description: List users based on filter
    Usecases:
      - Enumerate kerberoastable users
    Function: Domain
    Comments:
      - 'PowerShell Module: `ActiveDirectory`'
    MitreAttack:
  - Command: Get-ADUser -Filter {TrustedForDelegation -eq $true}
    Description: List users based on filter
    Usecases:
      - Enumerate accounts that are trusted for unconstrained delegation
    Function: Domain
    Comments:
      - 'PowerShell Module: `ActiveDirectory`'
    MitreAttack:
  - Command: 'Get-ADUser -LDAPFilter "(adminCount=1)" -Server ad.bitsadmin.com'
    Description: List users based on LDAP filter
    Usecases:
      - Enumerate users which [have been/are] members of at least one Administrative group
    Function: Domain
    Comments:
      - 'PowerShell Module: `ActiveDirectory`'
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
