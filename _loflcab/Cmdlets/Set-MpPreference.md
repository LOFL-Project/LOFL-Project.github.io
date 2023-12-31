---
Name: Set-MpPreference
Description: Configures preferences for Windows Defender scans and updates
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Set-MpPreference -CimSession $s -DisableRealtimeMonitoring $true
    Description: Disable realtime monitoring
    Usecases:
      - Disable the realtime protection of Windows Defender to be able to drop malicious binaries
    Function: Manage
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - Note this will shown an alert to the user, alternative is to add an excluded folder using [Add-MpPreference](../Add-MpPreference)
      - 'PowerShell Module: `Defender`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
