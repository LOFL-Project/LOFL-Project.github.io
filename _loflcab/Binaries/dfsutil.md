---
Name: dfsutil.exe
Description: Manage DFS Namespaces, servers, and clients
Updated: 2023-07-01
Toolsets:
  - RSAT
Commands:
  - Command: dfsutil.exe root \\ad.bitsadmin.com\Users
    Description: List DFS servers of namespace
    Usecases:
    Function: Data
    Comments:
      - 'Obtains the information from the DC via port 445/TCP -> DCE/RPC -> Settings for Microsoft Distributed File System'
      - Performs (many) resolves via DNS.
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
