---
Name: Get-DhcpServerv4FilterList
Description: Gets the enabled state of the allow filter list and deny filter list set on the Dynamic Host Configuration Protocol (DHCP) server service
Updated: 2023-07-01
Toolsets:
  - CIMSession
  - TODO
Commands:
  - Command: Get-DhcpServerv4FilterList -CimSession $s
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
