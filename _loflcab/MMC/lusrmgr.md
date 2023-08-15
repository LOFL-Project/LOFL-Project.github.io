---
Name: lusrmgr.msc
Description: Local Users and Groups
Updated: 2023-07-01
Toolsets:
  - Builtin
  - GUI
Commands:
  - Command: lusrmgr.msc /computer=W10.ad.bitsadmin.com
    Description: Local Users and Groups
    Usecases:
      - Add a backdoor user
      - Change password of existing user
      - Enable and disable accounts
      - Add users to, and remove users from groups
    Function: Manage
    Comments:
      - Alternative is to use [compmgmt.msc](../compmgmt)
    MitreAttack:
      - T1531
      - T1136.001
      - T1078.003
Resources:
Detections:
  - Port: 445/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---