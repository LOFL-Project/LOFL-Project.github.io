---
Name: Get-MpComputerStatus
Description: Gets the status of antimalware software on the computer
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Get-MpComputerStatus -CimSession $s
    Description: Check status of AV
    Usecases:
      - Identify whether the AV is active
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
