---
Name: Set-NetConnectionProfile
Description: Changes the network category of a connection profile
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Set-NetConnectionProfile -CimSession $s -InterfaceAlias 'Ethernet0' -NetworkCategory Private
    Description: Update connection profile for network adapter
    Usecases:
      - Update connection profile to have a different firewall policy applied
    Function: Network
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `NetConnection`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
