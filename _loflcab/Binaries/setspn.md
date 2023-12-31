---
Name: setspn.exe
Description: Reads, modifies, and deletes the Service Principal Names (SPN) directory property for an Active Directory service account
Updated: 2023-07-01
Toolsets:
  - Builtin
Commands:
  - Command: setspn.exe -L ad.bitsadmin.com\SP2019
    Description: List SPNs for a specific account
    Usecases:
      - Reconnaissance
    Function: Domain
    Comments:
      - Can be both a regular account as well as a computer account
    MitreAttack:
  - Command: setspn.exe -T ad.bitsadmin.com -Q */*
    Description: List all SPNs in the domain
    Usecases:
      - Reconnaissance
    Function: Domain
    Comments:
    MitreAttack:
  - Command: setspn.exe -S HTTP/EXCH2019.ad.bitsadmin.com EXCH2019
    Description: Set SPN
    Usecases:
      - Add an SPN to a user for a targeted Kerberoast
    Function: Domain
    Comments:
      - 'Error when execution from Offensive Windows VM: `Ldap Error(0x51 -- Server Down): ldap_connect; Failed to retrieve DN for domain "" : 0x00000051; Warning: No valid targets specified, reverting to current domain.; FindDomainForAccount: Call to DsGetDcNameWithAccountW failed with return value 0x0000054B; Unable to locate account SP2019`'
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
