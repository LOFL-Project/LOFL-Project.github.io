---
Name: nslookup.exe
Description: Displays information that you can use to diagnose Domain Name System (DNS) infrastructure
Updated: 2023-07-01
Toolsets:
  - Builtin
Commands:
  - Command: nslookup.exe -q=srv _ldap._tcp.ad.bitsadmin.com
    Description: List LDAP servers
    Usecases:
      - Identify DC IPs
    Function: Network
    Comments:
      - For more DNS domain-related DNS queries, see the link in the resources on DNS-Based Discovery
    MitreAttack:
      - T1590.002
Resources:
  - https://learn.microsoft.com/en-us/openspecs/windows_protocols/ms-adts/7fcdce70-5205-44d6-9c3a-260e616a2f04
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
