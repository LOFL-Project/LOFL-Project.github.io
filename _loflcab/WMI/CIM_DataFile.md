---
Name: CIM_DataFile
Description: Type of logical file that is a named collection of data or executable code
Updated: 2024-12-13
Toolsets:
  - Builtin
  - CIMSession
Commands:
  - Command: 'Get-CimInstance -Query "Select * from CIM_DataFile Where ((Drive = ''C:'') AND (FileName = ''ntuser'') AND (Extension = ''dat''))" -CimSession $s'
    Description: Locate files
    Usecases: Perform reconaissance on filesystem
    Function: Data
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
      - Pretty slow
      - 'Namespace: `ROOT\Cimv2`'
    MitreAttack:
  - Command: |
      $f = Get-CimInstance -ClassName CIM_DataFile -Filter "Name='C:\\Unattend.xml'" -CimSession $s
      $f | Invoke-CimMethod -Name Copy -Arguments @{FileName='C:\\Users\\Public\\Unattend.xml'}
    Description: Copy file
    Usecases: Copy file to Public share to copy it from there
    Function: Data
    Comments:
      - 'Create CimSession `$s` using [New-CimSession](../../Cmdlets/New-CimSession/)'
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
