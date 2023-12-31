---
Name: Get-NetEventSession
Description: Gets network event sessions
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Get-NetEventSession -Name sess -CimSession $s
    Description: Get status of an event session
    Usecases:
      - Sniff authentication traffic on a domain controller and locally crack the hashes
    Function: Network
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - See all details in [New-NetEventSession](../New-NetEventSession)
      - 'PowerShell Module: `NetEventPacketCapture`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
