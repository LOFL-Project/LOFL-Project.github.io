---
Name: Dismount-DiskImage
Description: Dismounts a disk image (virtual hard disk or ISO) so that it can no longer be accessed as a disk
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
  - TODO
Commands:
  - Command: Dismount-DiskImage -CimSession $s
    Description: TODO
    Usecases:
    Function: Data
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `Storage`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
