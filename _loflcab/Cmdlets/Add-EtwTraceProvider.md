---
Name: Add-EtwTraceProvider
Description: Adds an ETW trace provider to an ETW Autologger configuration or ETW session
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
  - TODO
Commands:
  - Command: Add-EtwTraceProvider -CimSession $s
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
