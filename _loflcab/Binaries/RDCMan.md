---
Name: RDCMan.exe
Description: Remote Desktop Connection Manager
Updated: 2024-12-13
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
      - See also [mstsc.exe](../mstsc)
    MitreAttack:
      - T1021.001
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
