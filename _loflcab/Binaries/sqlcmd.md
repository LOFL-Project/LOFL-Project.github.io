---
Name: sqlcmd.exe
Description: Integrated environment for managing any SQL infrastructure, from SQL Server to Azure SQL Database
Updated: 2023-07-01
Toolsets:
  - Extra
Commands:
  - Command: sqlcmd.exe -S SQL1.ad.bitsadmin.com\SQLEXPRESS
    Description: SQL Server Command Line Tool
    Usecases:
      - 'Connect to MSSQL database and execute commands on the underlying OS using the `xp_cmdshell` stored procedure, execute CLR code or pivot over MSSQL server links'
    Function: Manage
    Comments:
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
