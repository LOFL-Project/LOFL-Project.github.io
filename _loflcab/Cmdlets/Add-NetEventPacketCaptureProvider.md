---
Name: Add-NetEventPacketCaptureProvider
Description: Adds a Remote Packet Capture provider
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Add-NetEventPacketCaptureProvider -SessionName sess -CimSession $s -Level 4 -CaptureType Physical
    Description: Add packet capture provider to eventsession
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