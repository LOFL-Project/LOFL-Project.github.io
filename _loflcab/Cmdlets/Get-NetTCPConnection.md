---
Name: Get-NetTCPConnection
Description: Gets TCP connections
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Get-NetTCPConnection -CimSession $s -State Listen
    Description: Enumerate listening TCP ports
    Usecases:
      - Recon on listening services
    Function: Network
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `NetTCPIP`'
    MitreAttack:
      - T1047
  - Command: Get-NetTCPConnection -CimSession $s -State Established
    Description: List established connections
    Usecases:
      - Recon on current network and Internet activity
    Function: Network
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - 'PowerShell Module: `NetTCPIP`'
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
