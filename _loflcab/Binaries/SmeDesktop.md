---
Name: SmeDesktop.exe
Description: Windows Admin Center
Updated: 2023-08-25
Toolsets:
  - Extra
  - GUI
Commands:
  - Command: '"C:\Program Files\Windows Admin Center\SmeDesktop.exe"'
    Description: Manage machines
    Usecases:
      - Manage Certificates, Devices, Events, Files & file sharing, Firewall, Installed apps, Local users & groups, Networks, Performance Monitor, PowerShell, Processes, Registry, Remote Desktop, Roles & features, Scheduled tasks, Services, Storage, Storage Migration Service, Storage Replica, System Insights and Updates
    Function: Manage
    Comments:
      - Download and install Windows Admin Center and install it
      - Underlying extensively uses WinRM
    MitreAttack:
Resources:
  - https://www.microsoft.com/evalcenter/download-windows-admin-center
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
