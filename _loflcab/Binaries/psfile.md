---
Name: psfile.exe
Description: Lists or closes files opened remotely
Updated: 2023-07-01
Toolsets:
  - Sysinternals
  - TODO
Commands:
  - Command: psfile.exe -nobanner \\W10.ad.bitsadmin.com
    Description: List files opened remotely
    Usecases:
    Function: Data
    Comments:
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
