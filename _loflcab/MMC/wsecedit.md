---
Name: wsecedit.dll
Description: Security Configuration and Analysis
Updated: 2023-07-01
Toolsets:
  - Builtin
  - GUI
Commands:
  - Command: mmc.exe
    Description: Security Configuration and Analysis
    Usecases:
    Function: Manage
    Comments:
      - 'Open via MMC''s Add/Remove Snap-In -> Security Configuration and Analysis -> OK'
      - 'Right click the node -> Open Database -> Enter whatever name -> Open -> Open the .inf file'
    MitreAttack:
  - Command: mmc.exe
    Description: Security Templates
    Usecases:
    Function: Manage
    Comments:
      - 'Open via MMC''s Add/Remove Snap-In -> Security Configuration and Analysis -> OK'
      - Used to create .inf files from [secpol.msc](../secpol) settings
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
