---
Name: Get-DnsServer
Description: Retrieves a DNS server configuration
Updated: 2023-07-01
Toolsets:
  - CIMSession
  - RSAT
Commands:
  - Command: Get-DnsServer -CimSession $s
    Description: Show DNS server configuration
    Usecases:
    Function: Network
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `DnsServer`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
