---
Name: Stop-Computer
Description: Stops (shuts down) local and remote computers
Updated: 2023-07-01
Toolsets:
  - Builtin
Commands:
  - Command: Stop-Computer -ComputerName W10.ad.bitsadmin.com,w11.ad.bitsadmin.com -Force
    Description: Shutdown machines
    Usecases:
      - Make machine unavailable
    Function: Sessions
    Comments:
      - 'PowerShell Module: `Microsoft.PowerShell.Management`'
    MitreAttack:
      - T1529
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
