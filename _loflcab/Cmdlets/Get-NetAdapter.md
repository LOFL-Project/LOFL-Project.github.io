---
Name: Get-NetAdapter
Description: Gets the basic network adapter properties
Updated: 2024-12-13
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Get-NetAdapter -Name * -CimSession $s
    Description: List adapters
    Usecases:
      - Identify whether a machine is dual-homed
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
