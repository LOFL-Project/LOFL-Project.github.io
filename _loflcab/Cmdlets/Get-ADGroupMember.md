---
Name: Get-ADGroupMember
Description: Gets the members of an Active Directory group
Updated: 2023-07-01
Toolsets:
  - RSAT
Commands:
  - Command: 'Get-ADGroupMember "Domain Admins" -Recursive -Server ad.bitsadmin.com'
    Description: List all members of a group
    Usecases:
      - Understand interesting targets in the environment
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
