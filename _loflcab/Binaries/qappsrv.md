---
Name: qappsrv.exe
Description: Displays the available Remote Desktop Session Host servers on the network
Updated: 2024-12-13
Toolsets:
  - Builtin
Commands:
  - Command: qappsrv dc1.ad.bitsadmin.com
    Description: Display information about Remote Desktop Session Host server
    Usecases:
    Function: Manage
    Comments:
      - Equivalent to [query.exe](../query) termserver
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
