---
Name: New-ADComputer
Description: Creates a new Active Directory computer
Updated: 2023-07-01
Toolsets:
  - RSAT
Commands:
  - Command: |
      $account = 'MyComputer'
      $password = 'Password1!'
      $domain = 'ad.bitsadmin.com'
      New-ADComputer -Name $account -SAMAccountName $account -AccountPassword (ConvertTo-SecureString $password -Force -AsPlainText) -Verbose -DNSHostName "$account.$domain" -ServicePrincipalNames @("HOST/$account.$domain","RestrictedKrbHost/$account.$domain","HOST/$account","RestrictedKrbHost/$account")
    Description: Create computer account
    Usecases:
      - Create backdoor user in the AD
    Function: Domain
    Comments:
      - Can be performed by a regular user
      - 'By default the attribute `ms-DS-MachineAccountQuota` (global setting) is set to 10 for all domain users'
      - 'PowerShell Module: `ActiveDirectory`'
    MitreAttack:
      - T1136.002
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
