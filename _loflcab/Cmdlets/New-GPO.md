---
Name: New-GPO
Description: Creates a GPO
Updated: 2023-07-01
Toolsets:
  - RSAT
  - TODO
Commands:
  - Command: New-GPO -Name RunImmediateScheduledTask
    Description: Create new GPO
    Usecases:
      - Create new GPO which runs an immediate scheduled task to deploy an implant on the computers in the OU it is linked to
    Function: Domain
    Comments:
      - 'PowerShell Module: `GroupPolicy`'
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
