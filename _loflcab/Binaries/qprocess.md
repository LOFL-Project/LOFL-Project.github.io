---
Name: qprocess.exe
Description: Displays information about processes that are running on a Remote Desktop Session Host server
Updated: 2024-12-13
Toolsets:
  - Builtin
Commands:
  - Command: 'qprocess.exe /server:W10.ad.bitsadmin.com DomainUser2'
    Description: List all processes
    Usecases:
      - Reconnaissance on running processes for a specific user
    Function: Processes
    Comments:
    MitreAttack:
      - T1057
  - Command: 'qprocess.exe /server:W10.ad.bitsadmin.com *'
    Description: List all processes
    Usecases:
      - Reconnaissance on running processes
    Function: Processes
    Comments:
      - Equivalent to [query.exe](../query) process
    MitreAttack:
      - T1057
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
