---
Name: ServerManager.exe
Description: Manage roles and features on servers in the domain
Updated: 2023-07-01
Toolsets:
  - GUI
  - RSAT
Commands:
  - Command: ServerManager.exe
    Description: Server Manager
    Usecases:
      - Manage roles and features on servers
    Function: Manage
    Comments:
      - 'Add other servers to manage -> DNS -> `DC1.ad.bitsadmin.com` -> Enter -> Arrow -> OK'
    MitreAttack:
Resources:
Detections:
  - Port: 5985/TCP
  - Port: 5986/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
