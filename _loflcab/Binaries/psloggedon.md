---
Name: psloggedon.exe
Description: See who's logged on
Updated: 2023-07-01
Toolsets:
  - Sysinternals
Commands:
  - Command: psloggedon.exe -nobanner \\W10.ad.bitsadmin.com
    Description: List both interactive sessions and sessions to shares
    Usecases:
    Function: Sessions
    Comments:
    MitreAttack:
  - Command: psloggedon.exe \\W10.ad.bitsadmin.com
    Description: Show sessions
    Usecases:
      - Reconnaissance on currently active users
    Function: Sessions
    Comments:
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
