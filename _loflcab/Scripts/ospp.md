---
Name: ospp.vbs
Description: Configure volume licensed versions of Office products
Updated: 2023-07-01
Toolsets:
  - Extra
Commands:
  - Command: cscript.exe ospp.vbs W10.ad.bitsadmin.com /dstatusall
    Description: Show Office activation information
    Usecases:
    Function: Misc
    Comments:
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
