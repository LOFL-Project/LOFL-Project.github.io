---
Name: Microsoft.ConfigurationManagement.exe
Description: Microsoft Configuration Manager (MCM)
Updated: 2023-11-04
Toolsets:
  - Extra
  - GUI
Commands:
  - Command: '"C:\Program Files (x86)\Microsoft Endpoint Manager\AdminConsole\bin\Microsoft.ConfigurationManagement.exe"'
    Description: Manage Microsoft Configuration Manager (MCM)
    Usecases:
      - Collect information about systems
      - Deploy software implant to system
    Function: Manage
    Comments:
      - Download software, including Configuration Manager console on reference 1
      - Installation instructions on reference 2
      - 'At the Microsoft Configuration main screen, choose "Install Configuration Manager console"'
      - 'Add the `SMS:DebugView` parameter to the commandline to get an additional option (Tools) in the menu'
      - Formerly known as System Center Configuration Manager (SCCM)
    MitreAttack:
Resources:
  - https://www.microsoft.com/en-us/evalcenter/download-microsoft-endpoint-configuration-manager
  - https://learn.microsoft.com/en-us/mem/configmgr/core/servers/deploy/install/install-consoles
  - https://http418infosec.com/offensive-sccm-summary
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
