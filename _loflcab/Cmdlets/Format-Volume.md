---
Name: Format-Volume
Description: Formats one or more existing volumes or a new volume on an existing partition
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Format-Volume -CimSession $s -DriveLetter D -Force
    Description: Format volume
    Usecases:
      - Affect availability of data on a volume
    Function: Data
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `Storage`'
    MitreAttack:
      - T1485
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
