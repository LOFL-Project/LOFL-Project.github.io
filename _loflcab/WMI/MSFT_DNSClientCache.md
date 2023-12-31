---
Name: MSFT_DNSClientCache
Description: Represents a record in a DNS client cache
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Get-CimInstance -Namespace ROOT\StandardCimv2 -ClassName MSFT_DNSClientCache -CimSession $s
    Description: List cached DNS entries
    Usecases:
      - Reconnaissance on the network/Internet activities on the computer
    Function: Network
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - See also [Get-DnsClientCache](../../Cmdlets/Get-DnsClientCache)
      - 'Namespace: `ROOT\StandardCimv2`'
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
