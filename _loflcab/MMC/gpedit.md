---
Name: gpedit.msc
Description: Local Group Policy Editor
Updated: 2024-12-13
Toolsets:
  - Builtin
  - GUI
Commands:
  - Command: 'gpedit.msc /gpcomputer: DC1.ad.bitsadmin.com'
    Description: Local Group Policy Editor for a computer
    Usecases:
      - Add evil startup script
      - Weaken security as a backdoor
      - Open ports in the firewall
    Function: Manage
    Comments:
      - Quotes around the hostname or in case of no quotes a space before the hostname seem to be required
      - 'Through SMB edits files in `\\DC1.ad.bitsadmin.com\ADMIN$\GroupPolicy` (= `%SystemRoot%\System32\GroupPolicy`)'
    MitreAttack:
  - Command: 'gpedit.msc /gpobject:"LDAP://CN={31B2F340-016D-11D2-945F-00C04FB984F9},CN=Policies,CN=System,DC=ad,DC=bitsadmin,DC=com"'
    Description: Local Group Policy Editor for a computer
    Usecases:
      - Execute immediate scheduled tasks on machines to launch implant
    Function: Domain
    Comments:
      - Example edits Default Domain Policy, change GUID for editing other policies
      - 'Through SMB edits files in `\\ad.bitsadmin.com\SYSVOL\{GUID}` (= `%SystemRoot%\Sysvol\sysvol\ad.bitsadmin.com` by default) on the DC'
    MitreAttack:
      - T1037.003
      - T1484.001
Resources:
Detections:
  - Port: 445/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
