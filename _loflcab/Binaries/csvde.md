---
Name: csvde.exe
Description: Imports and exports data from Active Directory Domain Services (AD DS) using files that store data in the comma-separated value (CSV) format
Updated: 2023-07-01
Toolsets:
  - Builtin
  - TODO
Commands:
  - Command: 'csvde.exe -m -f users.csv -s DC1.ad.bitsadmin.com -d "cn=users,DC=ad,DC=bitsadmin,DC=com" -r "(objectClass=user)"'
    Description: Query all users
    Usecases:
      - Query LDAP over the commandline
    Function: Domain
    Comments:
      - Not sure if built-in
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
