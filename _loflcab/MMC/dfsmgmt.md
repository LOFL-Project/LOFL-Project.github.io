---
Name: dfsmgmt.msc
Description: DFS Management
Updated: 2023-07-01
Toolsets:
  - GUI
  - RSAT
Commands:
  - Command: dfsmgmt.msc
    Description: DFS Management
    Usecases:
    Function: Data
    Comments:
      - 'Right click root node -> Add Namespaces to Display or Add Replication Groups to Display'
    MitreAttack:
Resources:
Detections:
  - Port: 389/UDP
  - Port: 445/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
