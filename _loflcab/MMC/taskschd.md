---
Name: taskschd.msc
Description: Task Scheduler
Updated: 2023-11-04
Toolsets:
  - Builtin
  - GUI
Commands:
  - Command: taskschd.msc
    Description: Task Scheduler
    Usecases:
      - 'Create backdoor for persistence: Advantage, an EDR will have a hard time to connect the persistence to the implant/backdoor that is running the SOCKS server'
    Function: Execute
    Comments:
      - 'Right click -> Connect to Another Computer'
      - Alternatively, use [compmgmt.msc](../compmgmt)
    MitreAttack:
      - T1053.005
Resources:
Detections:
  - Port: 135/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
