---
Name: Close-SmbOpenFile
Description: Closes a file that is open by one of the clients of the SMB server
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
  - TODO
Commands:
  - Command: Close-SmbOpenFile -CimSession $s
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
