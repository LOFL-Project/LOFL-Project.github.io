---
Name: Get-NfsShare
Description: Gets NFS shares on an NFS server
Updated: 2023-07-01
Toolsets:
  - CIMSession
  - TODO
Commands:
  - Command: Get-NfsShare -CimSession $s
    Description: TODO
    Usecases:
    Function: Data
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: NFS'
    MitreAttack:
      - T1135
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
