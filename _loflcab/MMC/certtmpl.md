---
Name: certtmpl.msc
Description: Certificate Templates
Updated: 2023-07-01
Toolsets:
  - GUI
  - RSAT
Commands:
  - Command: certtmpl.msc
    Description: Certificate Templates
    Usecases:
      - Create new vulnerable templates and enroll for those as authentication backdoor
    Function: Manage
    Comments:
      - 'Right click root node -> Connect to another writable domain controller -> Change -> `ad.bitsadmin.com` -> OK'
      - Requires OffensiveDC
    MitreAttack:
Resources:
Detections:
  - Port: 389/UDP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
