---
Name: New-CimInstance
Description: Creates a CIM instance
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: 'New-CimInstance -ClassName Win32_Environment -Property @{Name="testvar";VariableValue="testvalue";UserName="<SYSTEM>"} -CimSession $s'
    Description: Create new instance
    Usecases:
      - Change PATH environment variable for search order hijacking
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
