---
Name: devcon.exe
Description: Displays detailed information about devices
Updated: 2023-07-01
Toolsets:
  - Extra
Commands:
  - Command: 'devcon.exe -m:\\W10.ad.bitsadmin.com find *'
    Description: List drivers
    Usecases:
      - Identify drivers of security solutions that are installed
    Function: Recon
    Comments:
      - Part of Tools component of Windows Driver Kit (WDK)
    MitreAttack:
      - TA0043
Resources:
  - https://learn.microsoft.com/en-us/windows-hardware/drivers/download-the-wdk
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
