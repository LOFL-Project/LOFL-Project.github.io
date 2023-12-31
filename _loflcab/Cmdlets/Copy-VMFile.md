---
Name: Copy-VMFile
Description: Copies a file to a virtual machine
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: 'Copy-VMFile -SourcePath C:\tmp\malware.exe -Name ''Windows 10 22H2'' -DestinationPath C:\Windows\System32\spoolsv64.exe -FileSource Host -CimSession $s'
    Description: Copy file to VM
    Usecases:
      - Copy implant to VM
    Function: Data
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - '`C:\tmp\malware.exe` is a file path on the Hyper-V host to which the `-CimSession $s` points'
      - '`malware.exe` can be copied to the Hyper-V host using [Copy-Item](../Copy-Item)'
      - Depends on some guest integration services to be enabled for the VM
      - 'PowerShell Module: `Hyper-V`'
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
