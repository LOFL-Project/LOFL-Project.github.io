---
Name: Get-ADObject
Description: Gets one or more Active Directory objects
Updated: 2023-07-01
Toolsets:
  - RSAT
Commands:
  - Command: 'Get-ADObject -Filter {msDS-AllowedToDelegateTo -ne "$null"} -Properties msDS-AllowedToDelegateTo, userAccountControl'
    Description: Query AD Objects using filter
    Usecases:
      - Enumerate users and computers with constrained delegation enabled
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
