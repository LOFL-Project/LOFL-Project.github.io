---
Name: Get-DfsnFolderTarget
Description: Gets settings for targets of a DFS namespace folder
Updated: 2023-07-01
Toolsets:
  - CIMSession
  - TODO
Commands:
  - Command: Get-DfsnFolderTarget -CimSession $s
    Description: TODO
    Usecases:
    Function: Data
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `DFSN`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
