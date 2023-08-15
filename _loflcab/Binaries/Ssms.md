---
Name: Ssms.exe
Description: SQL Server Management Studio (SSMS)
Updated: 2023-07-01
Toolsets:
  - Extra
  - GUI
Commands:
  - Command: ssms.exe
    Description: SQL Server Management Studio (SSMS)
    Usecases:
      - 'Connect to MSSQL database and execute commands on the underlying OS using the `xp_cmdshell` stored procedure, execute CLR code or pivot over MSSQL server links'
    Function: Manage
    Comments:
      - Download link in resources
      - See also [SQLServerManager15.msc](../../MMC/SQLServerManager15)
    MitreAttack:
Resources:
  - https://learn.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---