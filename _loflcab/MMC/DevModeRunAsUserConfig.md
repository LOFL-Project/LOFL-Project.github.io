---
Name: DevModeRunAsUserConfig.msc
Description: 'Group policy settings: Start Menu and Taskbar'
Updated: 2023-07-01
Toolsets:
  - Builtin
  - GUI
Commands:
  - Command: gpedit.msc
    Description: 'Group policy settings: Start Menu and Taskbar'
    Usecases:
    Function: Domain
    Comments:
      - For remote use, see [gpedit.msc](../gpedit)
      - 'Equivalent to gpedit.msc -> User Configuration -> Administrative Templates -> Start Menu and Taskbar'
    MitreAttack:
Resources:
Detections:
  - Port: 445/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
