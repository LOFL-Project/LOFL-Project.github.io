---
Name: gpme.msc
Description: Group Policy Management Editor
Updated: 2023-07-01
Toolsets:
  - GUI
  - RSAT
Commands:
  - Command: 'gpme.msc /gpobject:"LDAP://CN={31B2F340-016D-11D2-945F-00C04FB984F9},CN=Policies,CN=System,DC=ad,DC=bitsadmin,DC=com"'
    Description: Group Policy Management Editor
    Usecases:
      - Execute immediate scheduled tasks on machines to launch implant
    Function: Domain
    Comments:
      - Only possible from OffensiveDC
      - Commandline launches editor for the GUID of the default domain policy; can be changed to other GUIDs to edit different policies
    MitreAttack:
      - T1053.005
Resources:
Detections:
  - Port: 445/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
