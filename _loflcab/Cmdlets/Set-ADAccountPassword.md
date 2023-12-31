---
Name: Set-ADAccountPassword
Description: Modifies the password of an Active Directory account
Updated: 2023-07-01
Toolsets:
  - RSAT
Commands:
  - Command: |
      $new = ConvertTo-SecureString 'NewPassword1!' -A -F
      Set-ADAccountPassword -Identity MyAccount -Reset -NewPassword $new
    Description: Reset password
    Usecases:
      - Force reset a user's password to obtain access to the account
    Function: Domain
    Comments:
      - 'PowerShell Module: `ActiveDirectory`'
    MitreAttack:
      - T1531
  - Command: |
      $old = ConvertTo-SecureString 'OldPassword1!' -A -F
      $new = ConvertTo-SecureString 'NewPassword1!' -A -F
      Set-ADAccountPassword -Identity MyAccount -OldPassword $old -NewPassword $new
    Description: Update password
    Usecases:
      - Update a user's password
    Function: Domain
    Comments:
      - 'PowerShell Module: `ActiveDirectory`'
    MitreAttack:
      - T1531
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
