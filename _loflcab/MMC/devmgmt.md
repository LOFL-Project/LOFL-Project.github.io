---
Name: devmgmt.msc
Description: Device Manager
Updated: 2023-07-01
Toolsets:
  - Builtin
  - GUI
Commands:
  - Command: compmgmt.msc
    Description: Device Manager
    Usecases:
    Function: Manage
    Comments:
      - See [compmgmt.msc](../compmgmt) how to use it against a remote host. Returns errors though when connecting, so does not seem to work
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
