---
Name: Get-RemoteAccess
Description: Displays the configuration of DirectAccess (DA) and VPN (both Remote Access VPN and site-to-site VPN)
Updated: 2023-07-01
Toolsets:
  - CIMSession
  - TODO
Commands:
  - Command: Get-RemoteAccess -CimSession $s
    Description: TODO
    Usecases:
    Function: Processes
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: RemoteAccess'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
