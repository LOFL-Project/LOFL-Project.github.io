---
Name: Register-CimIndicationEvent
Description: Subscribes to indications using a filter expression or a query expression
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
  - TODO
Commands:
  - Command: Register-CimIndicationEvent -CimSession $s
    Description: TODO
    Usecases:
    Function: Execute
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
