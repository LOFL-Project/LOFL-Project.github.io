---
Name: RDCMan.exe
Description: Remote Desktop Connection Manager
Updated: 2023-07-01
Toolsets:
  - GUI
  - Sysinternals
Commands:
  - Command: RDCMan.exe
    Description: Remote Desktop
    Usecases:
    Function: Sessions
    Comments:
      - 'Session -> Connect To (Ctrl + Q) -> Enter server name'
    MitreAttack:
      - T1021.001
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
