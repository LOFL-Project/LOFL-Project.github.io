---
Name: tasklist.exe
Description: Displays a list of currently running processes
Updated: 2023-07-01
Toolsets:
  - Builtin
Commands:
  - Command: 'tasklist.exe /S W10.ad.bitsadmin.com /FO CSV > W10_tasklist.csv'
    Description: List processes
    Usecases:
      - Perform reconnaissance on executing processes
    Function: Processes
    Comments:
    MitreAttack:
      - T1057
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
