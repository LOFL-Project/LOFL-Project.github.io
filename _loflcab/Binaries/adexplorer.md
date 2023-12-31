---
Name: adexplorer.exe
Description: Advanced Active Directory (AD) viewer and editor
Updated: 2023-08-25
Toolsets:
  - GUI
  - Sysinternals
Commands:
  - Command: adexplorer.exe
    Description: Interactively browse LDAP
    Usecases:
      - 'Via File -> Connect, connect to a domain controller'
      - 'If adexplorer is running in the context of a domain, the "Connect to" field can be left empty as it automatically connects to a DC of the current domain'
      - When User and Password fields are left empty, Kerberos authentication is used
    Function: Domain
    Comments:
    MitreAttack:
  - Command: 'adexplorer.exe -snapshot ad.bitsadmin.com:636 ad.bitsadmin.com.dat'
    Description: Obtain dump of Active Directory over TLS
    Usecases:
      - Offline evaluation of the AD to identify vulnerabilities and attack paths
    Function: Domain
    Comments:
      - Can be viewed offline using ADExplorer
      - Can also be imported to BloodHound format using ADExplorerSnapshot.py or to Adalanche (see references)
    MitreAttack:
Resources:
  - https://blog.bitsadmin.com/dealing-with-large-bloodhound-datasets
  - https://github.com/c3c/ADExplorerSnapshot.py
  - https://github.com/lkarlslund/Adalanche
Detections:
  - Port: 389/TCP
  - Port: 636/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
