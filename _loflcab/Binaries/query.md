---
Name: query.exe
Description: Displays information about processes, sessions, and Remote Desktop Session Host servers
Updated: 2023-07-01
Toolsets:
  - Builtin
Commands:
  - Command: 'query.exe session /server:W10.ad.bitsadmin.com'
    Description: List listeners and interactive sessions
    Usecases:
      - Reconnaissance on currently active sessions
    Function: Sessions
    Comments:
    MitreAttack:
  - Command: 'query.exe user /server:W10.ad.bitsadmin.com'
    Description: List logged in users
    Usecases:
      - Reconnaissance on currently active users
    Function: Sessions
    Comments:
    MitreAttack:
  - Command: 'query.exe process /server:W10.ad.bitsadmin.com *'
    Description: List all processes
    Usecases:
      - Reconnaissance on running processes
    Function: Processes
    Comments:
    MitreAttack:
      - T1057
  - Command: 'query.exe process /server:W10.ad.bitsadmin.com keepass.exe'
    Description: List all processes
    Usecases:
      - Identify specific running process
    Function: Processes
    Comments:
    MitreAttack:
      - T1057
  - Command: query.exe termserver
    Description: List terminal servers on the network
    Usecases:
    Function: Sessions
    Comments:
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
