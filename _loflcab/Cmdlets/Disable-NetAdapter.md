---
Name: Disable-NetAdapter
Description: Disables a network adapter
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Disable-NetAdapter -Name Ethernet0 -CimSession $s
    Description: Disable network adapter
    Usecases:
      - Put remote machine offline
    Function: Network
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `NetAdapter`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
