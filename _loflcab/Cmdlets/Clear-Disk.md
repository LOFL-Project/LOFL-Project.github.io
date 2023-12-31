---
Name: Clear-Disk
Description: Cleans a disk by removing all partition information and un-initializing it, erasing all data on the disk
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Clear-Disk -CimSession $s -Number 3
    Description: Clear disk with id 3
    Usecases:
      - Affect availability of data on a disk
    Function: Data
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `Storage`'
    MitreAttack:
      - T1561
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
