---
Name: comexp.msc
Description: Component Services
Updated: 2024-04-19
Toolsets:
  - Builtin
  - GUI
Commands:
  - Command: comexp.msc
    Description: Component Services
    Usecases:
      - 'Privesc: manipulate settings of COM objects so it runs with higher privileges'
      - Modify ACLs to create a backdoor on the system
    Function: Manage
    Comments:
      - 'Component Services -> Computers -> Right click -> New -> Computer -> Browse -> `DC1.ad.bitsadmin.com`'
      - Does not work from OffensiveDC
      - 'Alternative way to launch: `dcomcnfg.exe`'
    MitreAttack:
Resources:
Detections:
  - Port: 135/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
