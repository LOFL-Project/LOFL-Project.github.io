---
Name: tsgateway.msc
Description: RD Gateway Manager
Updated: 2023-07-01
Toolsets:
  - GUI
  - RSAT
Commands:
  - Command: tsgateway.msc
    Description: RD Gateway Manager
    Usecases:
      - Disable auditing
      - Specify who can use the RD gateway and to which devices it can be used
    Function: Manage
    Comments:
      - 'Right click on RD Gateway Manager -> Connect to RD Gateway Server -> Remote server: `DC1.ad.bitsadmin.com`'
    MitreAttack:
Resources:
Detections:
  - Port: 135/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
