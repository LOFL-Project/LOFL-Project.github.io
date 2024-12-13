---
Name: scp.exe
Description: Secure Copy
Updated: 2024-12-13
Toolsets:
  - Builtin
Commands:
  - Command: scp.exe -o GSSAPIAuthentication=yes -o GSSAPIDelegateCredentials=yes myuser@linux.ad.bitsadmin.com:/tmp/file.tgz file.tgz
    Description: Copy file locally from SSH server authenticating using Kerberos
    Usecases:
      - Data collection
      - Tool transfer
    Function: Data
    Comments:
    MitreAttack:
      - T1105
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---