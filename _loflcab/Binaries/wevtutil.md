---
Name: wevtutil.exe
Description: Windows Events Command Line Utility
Updated: 2024-12-14
Toolsets:
  - Builtin
Commands:
  - Command: wevtutil /remote:CAROOT1.ad.bitsadmin.com cl Security
    Description: Clear security event log
    Usecases:
      - Cover tracks clearing past events
    Function: Recon
    Comments:
      - See also [Clear-EventLog](../../Cmdlets/Clear-Eventlog)
    MitreAttack:
      - T1070.001
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
