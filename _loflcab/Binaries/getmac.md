---
Name: getmac.exe
Description: Returns the media access control (MAC) address and list of network protocols associated with each address for all network cards in each computer
Updated: 2023-07-01
Toolsets:
  - Builtin
Commands:
  - Command: getmac.exe /V /S W10.ad.bitsadmin.com
    Description: List network adapters
    Usecases:
    Function: Network
    Comments:
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
