---
Name: reg.exe
Description: Query and edit the registry
Updated: 2023-07-01
Toolsets:
  - Builtin
Commands:
  - Command: 'reg.exe query "\\W10.ad.bitsadmin.com\HKLM\Software\Microsoft\Windows\CurrentVersion\Run"'
    Description: Query registry key
    Usecases:
      - Query registry autoruns
    Function: Registry
    Comments:
    MitreAttack:
      - T1012
      - T1547.001
  - Command: reg.exe add \\W10.ad.bitsadmin.com\HKLM\SYSTEM\CurrentControlSet\Control\Lsa /v DisableRestrictedAdmin /d 0 /t REG_DWORD
    Description: Set registry value
    Usecases:
      - Configure the remote system, e.g. to support Kerberos authentication for remote desktop
      - Configure the automatic start of an implant upon boot
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
