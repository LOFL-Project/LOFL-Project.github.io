---
Name: schmmgmt.dll
Description: Active Directory Schema
Updated: 2023-07-01
Toolsets:
  - GUI
  - RSAT
Commands:
  - Command: mmc.exe
    Description: Active Directory Schema
    Usecases:
    Function: Domain
    Comments:
      - 'Open via MMC''s Add/Remove Snap-in, then right click the root node -> Change Active Directory Domain Controller'
    MitreAttack:
Resources:
Detections:
  - Port: 389/UDP
  - Port: 445/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
