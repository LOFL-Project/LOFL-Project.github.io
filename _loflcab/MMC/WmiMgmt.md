---
Name: WmiMgmt.msc
Description: WMI Control
Updated: 2023-07-01
Toolsets:
  - Builtin
  - GUI
Commands:
  - Command: WmiMgmt.msc
    Description: WMI Control
    Usecases:
      - Add WMI backdoor by weakening the security of the root namespace
    Function: Manage
    Comments:
      - 'Right click WMI Control -> Connect to another computer -> Another computer: `DC1.ad.bitsadmin.com` -> OK'
    MitreAttack:
      - T1047
Resources:
Detections:
  - Port: 135/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
