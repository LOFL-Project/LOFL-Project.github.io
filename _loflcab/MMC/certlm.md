---
Name: certlm.msc
Description: Certificates - Local Computer
Updated: 2023-07-01
Toolsets:
  - Builtin
  - GUI
Commands:
  - Command: certlm.msc
    Description: Certificates - Local Computer
    Usecases:
      - Export private keys (if marked as exportable)
      - Install malicious trusted root certificates
    Function: Manage
    Comments:
      - 'Right click -> Connect to another computer -> Enter the object name to select -> `DC1.ad.bitsadmin.com`'
      - Quite slow when used over SOCKS
    MitreAttack:
      - T1553.004
Resources:
Detections:
  - Port: 445/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
