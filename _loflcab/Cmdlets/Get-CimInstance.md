---
Name: Get-CimInstance
Description: Gets the CIM instances of a class from a CIM server
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Get-CimInstance -CimSession $s -ClassName Win32_Process
    Description: Get instances of a CIM class
    Usecases:
      - List running processes
    Function: Processes
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `CimCmdlets`'
    MitreAttack:
      - T1047
  - Command: Get-CimInstance -ClassName Win32_Process | % { [PSCustomObject]@{Name=$_.Name; User=$(Invoke-CimMethod -InputObject $_ -MethodName GetOwner).User } }
    Description: Get instances of a CIM class
    Usecases:
      - List running processes including username
    Function: Processes
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `CimCmdlets`'
    MitreAttack:
      - T1047
  - Command: 'Get-CimInstance -Filter ''Name="TermService"'' -ClassName Win32_Service -CimSession $s'
    Description: Get instances of a CIM class
    Usecases:
      - 'Obtain the "Remote Desktop Services" service instance. This can now for example be used to launch or stop the service'
    Function: Manage
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `CimCmdlets`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
