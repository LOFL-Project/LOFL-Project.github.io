---
Name: psinfo.exe
Description: Local and remote system information viewer
Updated: 2023-07-01
Toolsets:
  - Sysinternals
Commands:
  - Command: psinfo.exe \\W10.ad.bitsadmin.com
    Description: Show basic information
    Usecases:
      - Reconnaissance on system information
    Function: Recon
    Comments:
      - Similar to [systeminfo.exe](../systeminfo)
    MitreAttack:
      - T1082
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
