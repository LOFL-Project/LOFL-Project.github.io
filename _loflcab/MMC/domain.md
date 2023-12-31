---
Name: domain.msc
Description: Active Directory Domains and Trusts
Updated: 2023-07-01
Toolsets:
  - GUI
  - RSAT
Commands:
  - Command: domain.msc /server=DC1.ad.bitsadmin.com
    Description: Active Directory Domains and Trusts
    Usecases:
      - Perform reconnaissance on domain trusts
    Function: Domain
    Comments:
      - Will initially show some errors because the offensive Windows host is not part of a domain
      - Right click the Active Directory Domains and Trusts node in the list of snap-ins and choose Change Forest or Change Domain. Now enter the FQDN of the root domain and click OK
    MitreAttack:
      - T1484.002
Resources:
Detections:
  - Port: 389/TCP
  - Port: 445/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
