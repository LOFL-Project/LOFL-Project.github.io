---
Name: tapimgmt.msc
Description: Telephony
Updated: 2023-07-01
Toolsets:
  - GUI
  - Server
Commands:
  - Command: tapimgmt.msc
    Description: Telephony
    Usecases:
    Function: Manage
    Comments:
      - 'Right click -> Add computer -> Another computer: `DC1.ad.bitsadmin.com` -> OK'
    MitreAttack:
Resources:
Detections:
  - Port: 445/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
