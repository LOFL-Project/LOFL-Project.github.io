---
Name: Win32_NTLogEvent
Description: Displays the Windows Event Log
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: 'Get-CimInstance -ClassName Win32_NTLogEvent -Filter "LogFile = ''Security'' AND EventCode = ''4624''" -CimSession $s'
    Description: List logons on a system
    Usecases:
      - Understand which accounts are used on a system
    Function: Logs
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
