---
Name: qwinsta.exe
Description: Display information about Remote Desktop Services sessions
Updated: 2023-07-01
Toolsets:
  - Builtin
Commands:
  - Command: 'qwinsta.exe /server:W10.ad.bitsadmin.com'
    Description: List listeners and interactive sessions
    Usecases:
      - Check whether the system has high-privileged users logged in to then laterally move to it
    Function: Sessions
    Comments:
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
