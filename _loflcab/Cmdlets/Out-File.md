---
Name: Out-File
Description: Sends output to a file
Updated: 2023-07-01
Toolsets:
  - Builtin
Commands:
  - Command: '"10.0.10.123 legit.com" | Out-File -Append \\W10.ad.bitsadmin.com\C$\Windows\System32\Drivers\etc\hosts -Encoding ascii'
    Description: Append line to file
    Usecases:
      - Add name to target host file to point to a malicious IP
    Function: Data
    Comments:
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
