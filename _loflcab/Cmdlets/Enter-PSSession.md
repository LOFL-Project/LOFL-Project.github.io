---
Name: Enter-PSSession
Description: Starts an interactive session with a remote computer
Updated: 2023-08-25
Toolsets:
  - Builtin
  - PSSession
Commands:
  - Command: Enter-PSSession -Session $ps
    Description: Start interactive session
    Usecases:
      - Launch shell and perform reconnaissance or install a backdoor
    Function: Execute
    Comments:
      - 'Create `$ps` using [New-PSSession](../New-PSSession)'
    MitreAttack:
      - T1021.006
  - Command: Enter-PSSession -ComputerName W10.ad.bitsadmin.com
    Description: Start interactive session
    Usecases:
      - Launch shell and perform reconnaissance or install a backdoor
    Function: Execute
    Comments:
    MitreAttack:
      - T1021.006
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
