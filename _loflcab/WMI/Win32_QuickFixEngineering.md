---
Name: Win32_QuickFixEngineering
Description: Represents a small system-wide update, commonly referred to as a quick-fix engineering (QFE) update, applied to the current operating system
Updated: 2023-07-01
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: Get-CimInstance Win32_QuickFixEngineering -CimSession $s
    Description: List of installed KBs
    Usecases:
      - List OS info and installed security updates and feed them to WES-NG to identify vulnerabilities
    Function: Recon
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - See also [systeminfo.exe](../../Binaries/systeminfo)
      - 'Namespace: `ROOT\Cimv2`'
    MitreAttack:
      - TA0043
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
