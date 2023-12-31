---
Name: Get-DnsClientCache
Description: Retrieves the contents of the DNS client cache
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Get-DnsClientCache -CimSession $s
    Description: List cached DNS entries
    Usecases:
      - Reconnaissance on the network/Internet activities on the computer
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
