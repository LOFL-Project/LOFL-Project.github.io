---
Name: Get-GPOReport
Description: Generates a report either in XML or HTML format for a specified GPO or for all GPOs in a domain
Updated: 2023-07-01
Toolsets:
  - Builtin
  - RSAT
  - TODO
Commands:
  - Command: 'Get-GPOReport -All -Domain ad.bitsadmin.com -Server DC1.ad.bitsadmin.com -ReportType Html -Path "$pwd\domain.html"'
    Description: Get report in HTML
    Usecases:
      - Information on group policies
    Function: Domain
    Comments:
      - 'PowerShell Module: `GroupPolicy`'
    MitreAttack:
  - Command: 'Get-GPOReport -All -Domain ad.bitsadmin.com -Server DC1.ad.bitsadmin.com -ReportType Xml -Path "$pwd\domain.xml"'
    Description: Get report in XML
    Usecases:
      - Information on group policies
    Function: Domain
    Comments:
      - 'PowerShell Module: `GroupPolicy`'
    MitreAttack:
  - Command: Get-GPOReport
    Description: TODO
    Usecases:
    Function: Domain
    Comments:
      - 'PowerShell Module: `GroupPolicy`'
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
