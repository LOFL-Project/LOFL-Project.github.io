---
Name: srvinfo.exe
Description: Gather information about a target server
Updated: 2023-07-01
Toolsets:
  - Extra
Commands:
  - Command: srvinfo.exe \\DC1.ad.bitsadmin.com
    Description: List computer information
    Usecases:
      - List OS info and installed security updates and feed them to WES-NG to identify vulnerabilities
    Function: Recon
    Comments:
      - Similar to [systeminfo.exe](../systeminfo)
      - Part of the Windows Server 2003 Resource Kit
    MitreAttack:
      - T1082
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
