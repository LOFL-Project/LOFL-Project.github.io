---
Name: uptime.exe
Description: Display uptime of a system
Updated: 2023-07-01
Toolsets:
  - Extra
Commands:
  - Command: uptime.exe W10.ad.bitsadmin.com
    Description: Show uptime
    Usecases:
      - Identify if a machine could be relevant for longer term persistence without having to install persistence
    Function: Recon
    Comments:
    MitreAttack:
      - T1082
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
