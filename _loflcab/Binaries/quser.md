---
Name: quser.exe
Description: Displays information about user sessions on a Remote Desktop Session Host server
Updated: 2024-12-13
Toolsets:
  - Builtin
Commands:
  - Command: 'quser.exe /server:W10.ad.bitsadmin.com'
    Description: List logged in users
    Usecases:
      - Check whether the system has high-privileged users logged in to then laterally move to it
    Function: Sessions
    Comments:
      - Equivalent to [query.exe](../query) user
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
