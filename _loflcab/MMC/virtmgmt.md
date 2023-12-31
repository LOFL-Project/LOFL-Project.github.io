---
Name: virtmgmt.msc
Description: Hyper-V Manager
Updated: 2023-07-01
Toolsets:
  - GUI
  - RSAT
Commands:
  - Command: virtmgmt.msc
    Description: Hyper-V Manager
    Usecases:
      - 'Connect to the console of a server which might be directly accessible because of an `AutoAdminLogon` registry setting, or because an admin has logged onto the console'
      - Install an unmonitored offensive VM to use to pivot through the network
    Function: Manage
    Comments:
      - 'Right click root node -> Connect to Server -> Remote server -> `HYPERV1.ad.bitsadmin.com`'
      - Uses ports 5985/TCP (WinRM, for management and non-enhanced session) and 2197/TCP (VMRDP for Enhanced Session) - Once a VM screen is opened (little display appears to be rendered over WinRM)
      - If a screen is opened without using the enhanced session functionality, it continues to use WinRM
    MitreAttack:
Resources:
Detections:
  - Port: 5985/TCP
  - Port: 2197/TCP
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
