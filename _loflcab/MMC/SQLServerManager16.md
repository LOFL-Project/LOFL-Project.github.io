---
Name: SQLServerManager16.msc
Description: SQL Server 2022 Configuration Manager
Updated: 2023-07-01
Toolsets:
  - Extra
  - GUI
Commands:
  - Command: 'SQLServerManager16.msc /computer:SQL1.ad.bitsadmin.com'
    Description: SQL Server 2022 Configuration Manager
    Usecases:
    Function: Manage
    Comments:
      - 'Install "Integration Services" in the SQL Server Express or Developer installation wizard'
    MitreAttack:
Resources:
  - https://www.microsoft.com/en-us/evalcenter/download-sql-server-2022
Detections:
  - Port: 135/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
