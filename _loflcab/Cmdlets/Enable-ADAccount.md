---
Name: Enable-ADAccount
Description: Enables an Active Directory account
Updated: 2023-07-01
Toolsets:
  - RSAT
Commands:
  - Command: Enable-ADAccount
    Description: Enable account
    Usecases:
      - (Re-)enable account to make use of it
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
