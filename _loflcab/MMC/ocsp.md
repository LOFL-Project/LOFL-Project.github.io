---
Name: ocsp.msc
Description: Online Responder Management
Updated: 2023-07-01
Toolsets:
  - GUI
  - RSAT
Commands:
  - Command: 'ocsp.msc /Computer:DC1.ad.bitsadmin.com'
    Description: Online Responder Management
    Usecases:
    Function: Manage
    Comments:
      - 'Alternative via GUI: Right click Online Responder -> Retarget Responder -> Another computer: `DC1.ad.bitsadmin.com` -> OK'
    MitreAttack:
Resources:
Detections:
  - Port: 135/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
