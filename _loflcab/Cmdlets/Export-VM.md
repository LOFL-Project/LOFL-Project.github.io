---
Name: Export-VM
Description: Exports a virtual machine to disk
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: 'Export-VM -Name ''Windows 10 22H2'' -Path C:\tmp -CimSession $s'
    Description: Export VM
    Usecases:
      - Export a (running) VM and copy its data over the network
    Function: Manage
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - Can also be a running VM
      - Next, using [Copy-Item](../Copy-Item) the exported VM can be copied
      - 'PowerShell Module: `Hyper-V`'
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
