---
Name: Search-ADAccount
Description: Gets Active Directory user, computer, or service accounts
Updated: 2023-07-01
Toolsets:
  - RSAT
Commands:
  - Command: Search-ADAccount -AccountInactive -TimeSpan 30
    Description: Search for accounts
    Usecases:
      - Accounts that are inactive for at least 30 days
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
