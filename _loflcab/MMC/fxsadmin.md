---
Name: fxsadmin.msc
Description: Fax Service Manager
Updated: 2023-07-01
Toolsets:
  - GUI
  - Server
Commands:
  - Command: fxsadmin.msc
    Description: Fax Service Manager
    Usecases:
    Function: Manage
    Comments:
      - '`mmc.exe` -> File -> Add/Remove Snap-In -> Fax Service Manager -> Add -> Another computer: `DC1.ad.bitsadmin.com` -> Finish -> OK'
    MitreAttack:
Resources:
Detections:
  - Port: 445/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
