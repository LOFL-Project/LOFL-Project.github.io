---
Name: Get-MpPreference
Description: Gets preferences for the Windows Defender scans and updates
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Get-MpPreference -CimSession $s
    Description: Obtain the AV's configuration
    Usecases:
      - Identify whether the AV is active and which exclusion paths are configured
    Function: Recon
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `Defender`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
