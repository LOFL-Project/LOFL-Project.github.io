---
Name: azman.msc
Description: Authorization Manager
Updated: 2023-07-01
Toolsets:
  - GUI
  - RSAT
Commands:
  - Command: azman.msc
    Description: Authorization Manager
    Usecases:
    Function: Manage
    Comments:
      - 'Right click root node -> Open Authorization Store -> Active Directory or Active Directory Application Mode (ADAM) -> Browse'
    MitreAttack:
Resources:
Detections:
  - Port: 389/UDP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
