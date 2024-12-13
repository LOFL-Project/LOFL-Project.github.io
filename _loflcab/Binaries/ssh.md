---
Name: ssh.exe
Description: Secure Shell client
Updated: 2024-12-13
Toolsets:
  - Builtin
Commands:
  - Command: ssh.exe -Kv myuser@linux.ad.bitsadmin.com
    Description: Connect to SSH server using Kerberos
    Usecases:
      - Lateral movement
    Function: Sessions
    Comments:
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---