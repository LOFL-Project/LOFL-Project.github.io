---
Name: New-ADUser
Description: Creates a new Active Directory user
Updated: 2023-07-01
Toolsets:
  - RSAT
Commands:
  - Command: 'New-ADUser -Name "Backdoor" -AccountPassword (ConvertTo-SecureString "MyPassword!" -Force -AsPlainText) -Enabled $true'
    Description: Create new user
    Usecases:
      - Create backdoor user in the AD
    Function: Domain
    Comments:
      - 'PowerShell Module: `ActiveDirectory`'
    MitreAttack:
      - T1136.002
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
