---
Name: cusrmgr.exe
Description: Manage local user accounts
Updated: 2023-07-01
Toolsets:
  - Extra
Commands:
  - Command: cusrmgr.exe -u TargetUser -P Password1! -m \\W10.ad.bitsadmin.com
    Description: Update password
    Usecases:
      - Backdoor account
    Function: Manage
    Comments:
      - Part of the Windows 2000 Resource Kit
    MitreAttack:
  - Command: cusrmgr.exe -u TargetUser -alg Administrators -m \\W10.ad.bitsadmin.com
    Description: Add user to local Administrators group
    Usecases:
      - Backdoor account
    Function: Manage
    Comments:
      - Part of the Windows 2000 Resource Kit
    MitreAttack:
  - Command: cusrmgr.exe -u TargetUser -d -m \\W10.ad.bitsadmin.com
    Description: Delete user
    Usecases:
      - Clear tracks
    Function: Manage
    Comments:
      - Part of the Windows 2000 Resource Kit
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
