---
Name: systeminfo.exe
Description: Displays detailed configuration information about a computer and its operating system, including operating system configuration, security information, product ID, and hardware properties
Updated: 2023-08-25
Toolsets:
  - Builtin
Commands:
  - Command: systeminfo.exe /S W10.ad.bitsadmin.com
    Description: Show system information
    Usecases:
      - List OS info and installed security updates and feed them to WES-NG to identify vulnerabilities
    Function: Recon
    Comments:
    MitreAttack:
      - T1082
Resources:
  - https://blog.bitsadmin.com/windows-security-updates-for-hackers
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
