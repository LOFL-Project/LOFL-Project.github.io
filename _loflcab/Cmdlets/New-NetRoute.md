---
Name: New-NetRoute
Description: Creates a route in the IP routing table
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
  - TODO
Commands:
  - Command: New-NetRoute -CimSession $s
    Description: TODO
    Usecases:
    Function: Network
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `NetTCPIP`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
