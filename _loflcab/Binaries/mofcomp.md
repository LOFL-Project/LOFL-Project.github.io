---
Name: mofcomp.exe
Description: Parses a file containing MOF statements and adds the classes and class instances defined in the file to the WMI repository
Updated: 2023-07-01
Toolsets:
  - Builtin
  - TODO
Commands:
  - Command: 'mofcomp.exe -N:\\W10.ad.bitsadmin.com\root\subscription .\backdoor.mof'
    Description: Create persistence
    Usecases:
    Function: Execute
    Comments:
    MitreAttack:
      - T1047
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
