---
Name: psgetsid.exe
Description: Translates SIDs to names and vice versa
Updated: 2023-07-01
Toolsets:
  - Sysinternals
Commands:
  - Command: psgetsid.exe \\W10.ad.bitsadmin.com
    Description: Resolve computer SID
    Usecases:
    Function: Recon
    Comments:
      - Installs service on remote system
    MitreAttack:
      - TA0043
  - Command: psgetsid.exe \\W10.ad.bitsadmin.com Administrator
    Description: Resolve SID of user
    Usecases:
    Function: Recon
    Comments:
      - Installs service on remote system
    MitreAttack:
      - TA0043
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
