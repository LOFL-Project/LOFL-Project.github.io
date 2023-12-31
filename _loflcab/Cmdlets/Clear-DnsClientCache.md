---
Name: Clear-DnsClientCache
Description: Clears the contents of the DNS client cache
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Clear-DnsClientCache -CimSession $s
    Description: Clear DNS cache
    Usecases:
      - Clear the DNS cache from any DNS entries that the attacker might have (accidentally) placed there
    Function: Network
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `DnsClient`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
