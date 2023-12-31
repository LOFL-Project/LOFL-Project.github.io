---
Name: Get-ScheduledTask
Description: Gets the task definition object of a scheduled task that is registered on the local computer
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: 'Get-ScheduledTask -CimSession $s | % { [PSCustomObject]@{State=$_.State; TaskName=$_.TaskName; TaskPath=$_.TaskPath; Actions=$($a=$_.Actions;$($a.Id,$a.WorkingDirectory,$a.Execute,$a.Arguments).Where({$_ -ne $null}) -join " "); Author=$_.Author; Description=$_.Description; SecurityDescriptor=$_.SecurityDescriptor } }'
    Description: List details on scheduled tasks
    Usecases:
      - Reconnaissance
    Function: Processes
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
