---
Name: shrpubw.exe
Description: Create a Shared Folder Wizard
Updated: 2024-12-13
Toolsets:
  - Builtin
  - GUI
Commands:
  - Command: 'shrpubw /s W10.ad.bitsadmin.com'
    Description: Create a Shared Folder Wizard
    Usecases:
      - Add (hidden - dollar share) shared folder
    Function: Manage
    Comments:
      - Alternatively, use [fsmgmt.msc](../../MMC/fsmgmt)
    MitreAttack:
      - T1135
      - T1021.002
Resources:
Detections:
  - Port: 445/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
