---
Name: Microsoft.IdentityServer.msc
Description: AD FS Management
Updated: 2024-12-13
Toolsets:
  - GUI
  - Server
Commands:
  - Command: '%SystemRoot%\ADFS\Microsoft.IdentityServer.msc'
    Description: AD FS Management
    Usecases:
    Function: Manage
    Comments:
      - Seems not possible to use this MMC remotely. Use the ADFS PowerShell module instead
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
