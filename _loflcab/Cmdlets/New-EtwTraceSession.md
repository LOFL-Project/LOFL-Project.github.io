---
Name: New-EtwTraceSession
Description: Creates an ETW trace session
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
  - TODO
Commands:
  - Command: New-EtwTraceSession -CimSession $s
    Description: TODO
    Usecases:
    Function: Misc
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `EventTracingManagement`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
