---
Name: tsdiscon.exe
Description: Disconnects a session from a Remote Desktop Session Host (RD Session Host) server
Updated: 2023-07-01
Toolsets:
  - Builtin
Commands:
  - Command: 'tsdiscon.exe rdp-tcp#1 /server:W10.ad.bitsadmin.com'
    Description: Disconnect a user
    Usecases:
    Function: Sessions
    Comments:
    MitreAttack:
      - T1531
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
