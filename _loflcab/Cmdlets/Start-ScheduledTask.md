---
Name: Start-ScheduledTask
Description: Starts one or more instances of a scheduled task
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Start-ScheduledTask -CimSession $s -TaskName Backdoor
    Description: Launch scheduled task
    Usecases:
      - Launch implant
    Function: Execute
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `ScheduledTasks`'
    MitreAttack:
      - T1053.005
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
