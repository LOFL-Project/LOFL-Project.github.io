---
Name: winrm.cmd
Description: Windows Remote Management
Updated: 2023-07-01
Toolsets:
  - Builtin
Commands:
  - Command: 'winrm.vbs get wmicimv2/Win32_Process?Handle=3456 -r:W10.ad.bitsadmin.com'
    Description: Check process details
    Usecases:
      - Reconnaissance on running processes
    Function: Processes
    Comments:
    MitreAttack:
      - T1057
      - T1021.006
  - Command: 'winrm.vbs invoke Create wmicimv2/Win32_Process -r:W10.ad.bitsadmin.com @{CommandLine="notepad.exe";CurrentDirectory="C:\"}'
    Description: Lauch process
    Usecases:
      - After having copied an implant over SMB, launch it
    Function: Execute
    Comments:
    MitreAttack:
      - T1047
      - T1021.006
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
