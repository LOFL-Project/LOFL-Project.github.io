---
Name: Remove-SmbShare
Description: Deletes the specified SMB shares
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
  - TODO
Commands:
  - Command: Remove-SmbShare -CimSession $s
    Description: TODO
    Usecases:
    Function: Data
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `SmbShare`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
