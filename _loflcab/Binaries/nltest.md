---
Name: nltest.exe
Description: Perform network administrative tasks
Updated: 2023-07-01
Toolsets:
  - RSAT
Commands:
  - Command: 'nltest.exe /domain_trusts /all_trusts /v /server:DC1.ad.bitsadmin.com'
    Description: List domain trusts
    Usecases:
      - Understand the setup of the Active Directory forest
    Function: Domain
    Comments:
    MitreAttack:
  - Command: 'nltest.exe /SHUTDOWN:"" 0 /SERVER:W10.ad.bitsadmin.com'
    Description: Shutdown machine
    Usecases:
      - Make machine unavailable
    Function: Sessions
    Comments:
    MitreAttack:
      - T1529
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
