---
Name: Stop-EtwTraceSession
Description: Stops the specified ETW session
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
  - TODO
Commands:
  - Command: Stop-EtwTraceSession -CimSession $s
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
