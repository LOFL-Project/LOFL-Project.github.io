---
Name: Get-ADOrganizationalUnit
Description: Gets one or more Active Directory organizational units
Updated: 2023-07-01
Toolsets:
  - RSAT
Commands:
  - Command: Get-ADOrganizationalUnit 'OU=Domain Controllers,DC=ad,DC=bitsadmin,DC=com'
    Description: Obtain information about OU
    Usecases:
      - Learn which policies are applied to an OU
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
