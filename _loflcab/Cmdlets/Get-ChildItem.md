---
Name: Get-ChildItem
Description: Gets the files and folders in a file system drive.
Updated: 2023-08-25
Toolsets:
  - Builtin
Commands:
  - Command: 'Get-ChildItem -LiteralPath ''\\?\UNC\FS1.ad.bitsadmin.com\IT'' -Depth 25 -Force | ForEach-Object { [PSCustomObject]@{Name=$_.Name; Mode=$_.Mode; Length=$_.Length; LastWriteTime=$_.LastWriteTime.ToUniversalTime().ToString(''yyyy-MM-dd HH:mm:ss''); FullName=$_.FullName.Replace(''\?\UNC'','''') } } | Export-Csv -Encoding UTF8 -NoTypeInformation FS1_IT.csv'
    Description: Enumerate network share
    Usecases:
      - Create file listing of network share to identify files that can be used for escalation
    Function: Data
    Comments:
      - 'PowerShell Module: `Microsoft.PowerShell.Management`'
    MitreAttack:
      - T1083
Resources:
  - https://blog.bitsadmin.com/digging-for-secrets
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
