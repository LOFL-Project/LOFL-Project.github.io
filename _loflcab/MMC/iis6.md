---
Name: iis6.msc
Description: Internet Information Services (IIS) 6.0 Manager
Updated: 2023-07-01
Toolsets:
  - GUI
Commands:
  - Command: iis6.msc
    Description: Internet Information Services (IIS) 6.0 Manager
    Usecases:
    Function: Manage
    Comments:
      - 'Right click -> Connect -> Computer name: `DC1.ad.bitsadmin.com` -> OK'
    MitreAttack:
Resources:
Detections:
  - Port: 135/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
