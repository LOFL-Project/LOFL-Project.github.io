---
Name: AdRmsAdmin.msc
Description: Active Directory Rights Management Services
Updated: 2023-07-01
Toolsets:
  - GUI
  - RSAT
Commands:
  - Command: AdRmsAdmin.msc
    Description: Active Directory Rights Management Services
    Usecases:
    Function: Domain
    Comments:
      - 'Right click -> Add Cluster -> Connect to: Remote computer'
    MitreAttack:
Resources:
Detections:
  - Port: 80/TCP
  - Port: 443/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
