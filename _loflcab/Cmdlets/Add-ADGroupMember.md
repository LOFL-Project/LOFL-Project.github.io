---
Name: Add-ADGroupMember
Description: Adds one or more members to an Active Directory group
Updated: 2023-07-01
Toolsets:
  - RSAT
Commands:
  - Command: Add-ADGroupMember 'Domain Admins' -Members Hacker
    Description: Add user to domain group
    Usecases:
      - Add a user to a certain domain group to obtain certain privileges
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
