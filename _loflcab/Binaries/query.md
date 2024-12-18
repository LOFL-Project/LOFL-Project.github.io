---
Name: query.exe
Description: Displays information about processes, sessions, and Remote Desktop Session Host servers
Updated: 2024-12-13
Toolsets:
  - Builtin
Commands:
  - Command: 'query.exe session /server:W10.ad.bitsadmin.com'
    Description: List listeners and interactive sessions
    Usecases:
      - Reconnaissance on currently active sessions
    Function: Sessions
    Comments:
      - Equivalent to [qwinsta.exe](../qwinsta)
    MitreAttack:
  - Command: 'query.exe user /server:W10.ad.bitsadmin.com'
    Description: List logged in users
    Usecases:
      - Reconnaissance on currently active users
    Function: Sessions
    Comments:
      - Equivalent to [quser.exe](../quser)
    MitreAttack:
  - Command: 'query.exe process /server:W10.ad.bitsadmin.com *'
    Description: List all processes
    Usecases:
      - Reconnaissance on running processes
    Function: Processes
    Comments:
      - Equivalent to [qprocess.exe](../qprocess)
    MitreAttack:
      - T1057
  - Command: 'query.exe process /server:W10.ad.bitsadmin.com keepass.exe'
    Description: List all processes
    Usecases:
      - Identify specific running process
    Function: Processes
    Comments:
      - Equivalent to [qprocess.exe](../qprocess)
    MitreAttack:
      - T1057
  - Command: query.exe termserver
    Description: List terminal servers on the network
    Usecases:
    Function: Sessions
    Comments:
      - Equivalent to [qappsrv.exe](../qappsrv)
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
