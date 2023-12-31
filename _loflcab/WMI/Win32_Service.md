---
Name: Win32_Service
Description: Represents a service on a computer system running Windows
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: |
      $tssvc = Get-CimInstance -Filter 'Name="TermService"' -ClassName Win32_Service -CimSession $s
      $tssvc
      $tssvc | Invoke-CimMethod -MethodName StartService
    Description: Start service
    Usecases:
    Function: Execute
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'Namespace: `ROOT\Cimv2`'
    MitreAttack:
      - T1569.002
  - Command: Get-CimInstance -ClassName Win32_Service -CimSession $s
    Description: List services
    Usecases:
      - Reconnaissance on installed services
    Function: Processes
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
    MitreAttack:
  - Command: 'Get-CimInstance -Filter ''Name="TermService"'' -ClassName Win32_Service -CimSession $s'
    Description: Obtain a specific service instance
    Usecases:
      - Start or stop a service
    Function: Processes
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
    MitreAttack:
  - Command: 'Invoke-WmiMethod -Class Win32_Service -Name Create -ArgumentList $false,"Print Spooler (x64)",([byte]1),$null,$null,"spoolsv64","C:\Windows\System32\cmd.exe /c powershell -e bHM=",$null,([byte]16),"Manual","NT AUTHORITY\SYSTEM",""'
    Description: Create new service
    Usecases:
    Function: Execute
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
    MitreAttack:
      - TA0002
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
