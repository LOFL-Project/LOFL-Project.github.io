---
Name: nps.msc
Description: Network Policy Server
Updated: 2023-07-01
Toolsets:
  - GUI
  - Server
Commands:
  - Command: 'nps.msc /computer:DC1.ad.bitsadmin.com'
    Description: Network Policy Server
    Usecases:
    Function: Manage
    Comments:
      - 'Alternative: mmc.exe -> Add or Remove Snap-ins -> Network Policy Server -> Add -> Another computer -> `DC1.ad.bitsadmin.com` -> OK'
    MitreAttack:
Resources:
Detections:
  - Port: 445/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
