---
Name: Get-ADTrust
Description: Returns all trusted domain objects in the directory
Updated: 2023-07-01
Toolsets:
  - RSAT
Commands:
  - Command: Get-ADTrust -Filter * -Server ad.bitsadmin.com | ft Direction,Name,TrustType
    Description: Query AD trusts
    Usecases:
      - Understand trust relations of the forest and domains
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
