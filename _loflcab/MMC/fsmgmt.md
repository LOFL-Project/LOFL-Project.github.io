---
Name: fsmgmt.msc
Description: Shared Folders
Updated: 2023-07-01
Toolsets:
  - Builtin
  - GUI
Commands:
  - Command: 'fsmgmt.msc /computer:W10.ad.bitsadmin.com'
    Description: Shared Folders
    Usecases:
      - View which users are connected to the share from which computername
      - View which files are opened by which users
      - Add (hidden - dollar share) shared folder
    Function: Manage
    Comments:
      - Alternatively, use [compmgmt.msc](../compmgmt)
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
