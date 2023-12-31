---
Name: iis.msc
Description: Internet Information Services (IIS) Manager
Updated: 2023-07-01
Toolsets:
  - GUI
Commands:
  - Command: iis.msc
    Description: Internet Information Services (IIS) Manager
    Usecases:
      - Create virtual directory with web shell (drop shell over SMB or maybe create virtual directory on share)
      - Add FTP site to be able to browse the filesystem
      - Weaken authentication
      - Add MIME Types to be able to download certain file extensions
    Function: Manage
    Comments:
      - 'Right click Start Page -> Connect to a Server -> Server name: `SP2019.ad.bitsadmin.com` -> Next -> Enter User name/password -> Next -> Connection Name: `SP2019` -> Finish'
      - Requires to install and enabled Remote IIS Management service
      - Does not seem possible to perform authentication transparently through Kerberos
      - 'Can also be launched via `inetmgr.exe`'
    MitreAttack:
Resources:
  - https://woshub.com/remote-iis-management-in-windows-server-2012/
Detections:
  - Port: 8172/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
