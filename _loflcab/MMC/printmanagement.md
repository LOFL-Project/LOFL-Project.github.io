---
Name: printmanagement.msc
Description: Print Management
Updated: 2023-07-01
Toolsets:
  - Builtin
  - GUI
Commands:
  - Command: printmanagement.msc
    Description: Print Management
    Usecases:
      - Install a malicious printer driver?
    Function: Manage
    Comments:
    MitreAttack:
Resources:
Detections:
  - Port: 445/TCP
  - Port: 135/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
