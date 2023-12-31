---
Name: Get-NetIPAddress
Description: Gets the IP address configuration
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Get-NetIPAddress -CimSession $s | Sort InterfaceIndex | ft -Autosize InterfaceIndex, InterfaceAlias, AddressFamily, IPAddress, PrefixLength
    Description: List IP addresses of the various interfaces
    Usecases:
      - Identify whether a machine might be dual-homed
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
