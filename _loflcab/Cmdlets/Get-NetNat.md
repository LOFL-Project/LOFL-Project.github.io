---
Name: Get-NetNat
Description: Gets NAT objects
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
  - TODO
Commands:
  - Command: Get-NetNat -CimSession $s
    Description: TODO
    Usecases:
    Function: Network
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `NetNat`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---