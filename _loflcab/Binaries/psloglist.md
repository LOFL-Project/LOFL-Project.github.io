---
Name: psloglist.exe
Description: Dumps event logs on a local or remote system
Updated: 2023-07-01
Toolsets:
  - Sysinternals
Commands:
  - Command: psloglist.exe -nobanner -i 99999 -c \\W10.ad.bitsadmin.com Security
    Description: Clear Security event log
    Usecases:
      - Cover tracks clearing past logon events
    Function: Logs
    Comments:
      - Be aware that this leaves an event stating that the Security event log has been cleared (event id 1102)
    MitreAttack:
      - T1070.001
  - Command: psloglist.exe -nobanner -s \\W10.ad.bitsadmin.com Security
    Description: List events in the Security event log
    Usecases:
      - Identify which IPs logons of privileged users are originating from
    Function: Logs
    Comments:
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
