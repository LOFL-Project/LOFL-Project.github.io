---
Name: tskill.exe
Description: Ends a process
Updated: 2023-07-01
Toolsets:
  - Builtin
Commands:
  - Command: 'tskill.exe cmd /Server:W10.ad.bitsadmin.com /A /V'
    Description: Kill a process
    Usecases:
      - Terminate a process
    Function: Processes
    Comments:
    MitreAttack:
      - T1562.001
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
