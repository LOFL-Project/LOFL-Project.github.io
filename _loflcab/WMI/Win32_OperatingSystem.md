---
Name: Win32_OperatingSystem
Description: Represents a Windows-based operating system installed on a computer
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Get-CimInstance Win32_OperatingSystem -CimSession $s | fl *
    Description: Information about OS
    Usecases:
      - Reconnaissance of target operating system
    Function: Recon
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - See also [systeminfo.exe](../../Binaries/systeminfo)
      - 'Namespace: `ROOT\Cimv2`'
      - 'Alternative: `CIM_OperatingSystem`'
    MitreAttack:
      - TA0043
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
