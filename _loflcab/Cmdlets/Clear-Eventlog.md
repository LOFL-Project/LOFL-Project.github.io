---
Name: Clear-Eventlog
Description: Clears all entries from specified event logs on the local or remote computers.
Updated: 2024-12-13
Toolsets:
  - Builtin
Commands:
  - Command: Clear-EventLog -LogName Application,Security,System -ComputerName W10.ad.bitsadmin.com,W11.ad.bitsadmin.com
    Description: Clear various logs on various computers
    Usecases:
      - Cover tracks clearing past events in the various logs
    Function: Logs
    Comments:
      - Be aware that this leaves an event stating that the Security event log has been cleared (event id 1102)
      - See also [wevtutil.exe](../../Binaries/wevtutil)
    MitreAttack:
      - T1070.001
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
