---
Name: CluAdmin.msc
Description: Failover Cluster Manager
Updated: 2023-07-01
Toolsets:
  - GUI
  - RSAT
Commands:
  - Command: CluAdmin.msc
    Description: Failover Cluster Manager
    Usecases:
    Function: Manage
    Comments:
      - 'Right click Failover Cluster Manager -> Connect to Cluster -> Browse'
    MitreAttack:
Resources:
Detections:
  - Port: 389/UDP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
