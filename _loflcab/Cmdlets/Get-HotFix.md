---
Name: Get-HotFix
Description: Gets the hotfixes that are installed on local or remote computers
Updated: 2023-08-25
Toolsets:
  - Builtin
Commands:
  - Command: Get-HotFix -ComputerName W10.ad.bitsadmin.com
    Description: List installed KBs
    Usecases:
      - Feed them to Windows Exploit Suggester - Next Generation to identify what vulnerabilities the system is vulnerable to
    Function: Recon
    Comments:
      - 'PowerShell Module: `Microsoft.PowerShell.Management`'
    MitreAttack:
      - TA0043
Resources:
  - https://blog.bitsadmin.com/windows-security-updates-for-hackers
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
