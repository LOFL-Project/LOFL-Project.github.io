---
Name: mstsc.exe
Description: Connect to the desktop of remote computers
Updated: 2024-12-13
Toolsets:
  - Builtin
  - GUI
Commands:
  - Command: 'mstsc.exe /v:SP2019.ad.bitsadmin.com /shadow:1 /noConsentPrompt /control'
    Description: Control a user's session
    Usecases:
      - Take over when a user is idle
    Function: Sessions
    Comments:
    MitreAttack:
      - T1021.001
  - Command: 'mstsc.exe /remoteGuard /v:SP2019.ad.bitsadmin.com'
    Description: Remote Desktop
    Usecases:
      - Connect to a target server
      - 'Exfiltrate data over RDP clipboard or `\\tsclient` drives'
      - If RDP provides access to a different network segment, SocksOverRDP can be used to pivot into that segment
    Function: Sessions
    Comments:
      - See also [RDCMan.exe](../RDCMan)
    MitreAttack:
      - T1021.001
  - Command: 'mstsc.exe /v:SP2019.ad.bitsadmin.com /shadow:1 /noConsentPrompt'
    Description: Shadow a user
    Usecases:
      - Spy on a user's activity
    Function: Sessions
    Comments:
    MitreAttack:
      - T1021.001
Resources:
  - https://blog.bitsadmin.com/spying-on-users-using-rdp-shadowing
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
