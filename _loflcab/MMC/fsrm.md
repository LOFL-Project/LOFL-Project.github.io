---
Name: fsrm.msc
Description: File Server Resource Manager
Updated: 2023-07-01
Toolsets:
  - GUI
  - RSAT
Commands:
  - Command: fsrm.msc
    Description: File Server Resource Manager
    Usecases:
    Function: Manage
    Comments:
      - 'Right click File Server Resource Manager -> Connect to Another Computer -> Another computer: `DC1.ad.bitsadmin.com`'
    MitreAttack:
Resources:
Detections:
  - Port: 445/TCP
  - Port: 135/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
