---
Name: Get-DhcpServerSetting
Description: Gets the configuration parameters of the database of the Dynamic Host Configuration Protocol (DHCP) server service
Updated: 2023-07-01
Toolsets:
  - CIMSession
  - TODO
Commands:
  - Command: Get-DhcpServerSetting -CimSession $s
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
