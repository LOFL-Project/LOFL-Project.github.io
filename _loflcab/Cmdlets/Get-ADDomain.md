---
Name: Get-ADDomain
Description: Gets an Active Directory domain
Updated: 2023-07-01
Toolsets:
  - RSAT
Commands:
  - Command: Get-ADDomain ad.bitsadmin.com
    Description: Get domain
    Usecases:
      - Get information about the domain
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
