---
Name: gpresult.exe
Description: Displays the Resultant Set of Policy (RSoP) information for a remote user and computer
Updated: 2023-07-01
Toolsets:
  - Builtin
Commands:
  - Command: gpresult.exe /S W10.ad.bitsadmin.com /SCOPE COMPUTER /X W10.xml
    Description: Save effective policies to XML
    Usecases:
      - Understand group policies that are applicable
    Function: Recon
    Comments:
    MitreAttack:
      - TA0043
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
