---
Name: Get-DhcpServerDnsCredential
Description: Gets an account that the DHCP Server service uses to register or deregister client records on a DNS server
Updated: 2023-07-01
Toolsets:
  - CIMSession
  - TODO
Commands:
  - Command: Get-DhcpServerDnsCredential -CimSession $s
    Description: TODO
    Usecases:
    Function: Manage
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `DhcpServer`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
