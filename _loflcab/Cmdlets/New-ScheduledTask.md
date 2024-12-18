---
Name: New-ScheduledTask
Description: Creates a scheduled task instance
Updated: 2024-12-13
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: |
      $a = New-ScheduledTaskAction -Execute "C:\Tmp\backdoor.exe" -Argument '-background'
      $p = New-ScheduledTaskPrincipal -UserId "NT Authority\SYSTEM"
      $ss = New-ScheduledTaskSettingsSet -MultipleInstances Parallel -AllowStartIfOnBatteries -Compatibility Win8
      $d = New-ScheduledTask -CimSession $s -Action $a -Principal $p -Settings $ss
      $t = Register-ScheduledTask -CimSession $s Backdoor -InputObject $d
    Description: Create new scheduled task
    Usecases:
    Function: Execute
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - See [Register-ScheduledTask](../Register-ScheduledTask)
      - 'PowerShell Module: `ScheduledTasks`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
