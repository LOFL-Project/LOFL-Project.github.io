---
Name: Set-NetFirewallRule
Description: Modifies existing firewall rules
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
  - TODO
Commands:
  - Command: Set-NetFirewallRule -CimSession $s
    Description: TODO
    Usecases:
    Function: Network
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `netsecurity`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
