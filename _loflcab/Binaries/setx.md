---
Name: setx.exe
Description: Modifies the value of a service's entries in the registry and in the Service Control Manager database
Updated: 2023-07-01
Toolsets:
  - Builtin
Commands:
  - Command: 'setx.exe /S W10.ad.bitsadmin.com /M MYVAR "Hello there!"'
    Description: Set machine-wide environment variables
    Usecases:
      - Configure a path order hijack
    Function: Registry
    Comments:
    MitreAttack:
      - T1112
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
