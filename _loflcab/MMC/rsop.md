---
Name: rsop.msc
Description: Resultant Set of Policy
Updated: 2023-07-01
Toolsets:
  - Builtin
  - GUI
Commands:
  - Command: rsop.msc
    Description: Resultant Set of Policy
    Usecases:
      - Perform reconnaissance on applied (security) policies on remote system
    Function: Domain
    Comments:
      - 'Right click RSoP -> Change Query -> Another computer: `DC1.ad.bitsadmin.com` -> Next -> Next -> Next -> Finish'
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
