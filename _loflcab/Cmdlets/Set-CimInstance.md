---
Name: Set-CimInstance
Description: Modifies a CIM instance on a CIM server by calling the ModifyInstance method of the CIM class
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: 'Set-CimInstance -Query ''Select * from Win32_Environment where name LIKE "testvar%"'' -Property @{VariableValue="abcd"}'
    Description: Update attribute of CIM instance
    Usecases:
      - Update path variable
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
