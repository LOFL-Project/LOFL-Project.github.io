---
Name: Add-MpPreference
Description: Modifies settings for Windows Defender
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: 'Add-MpPreference -ExclusionPath ''C:\EvilTools'' -CimSession $s'
    Description: Exclude path from AV
    Usecases:
      - Exclude path from AV so malicious tools can be stored there
    Function: Manage
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
