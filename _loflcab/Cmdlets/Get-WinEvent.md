---
Name: Get-WinEvent
Description: Gets events from event logs and event tracing log files on local and remote computers
Updated: 2024-12-13
Toolsets:
  - Builtin
Commands:
  - Command: 'Get-WinEvent -ComputerName DC1.ad.bitsadmin.com -FilterHashtable @{logname="Security";id=4768} | % { [PSCustomObject]@{TimeCreated=$_.TimeCreated; TargetUserName=$_.Properties[0].Value; TargetDomainName=$_.Properties[1].Value; TargetSid=$_.Properties[2].Value; ServiceName=$_.Properties[3].Value; ServiceSid=$_.Properties[4].Value; TicketOptions=$_.Properties[5].Value; Status=$_.Properties[6].Value; TicketEncryptionType=$_.Properties[7].Value; PreAuthType=$_.Properties[8].Value; IpAddress=$_.Properties[9].Value; IpPort=$_.Properties[10].Value; CertIssuerName=$_.Properties[11].Value; CertSerialNumber=$_.Properties[12].Value; CertThumbprint=$_.Properties[13].Value} }'
    Description: List all Kerberos authentication requests
    Usecases:
      - Identify which IPs logons of privileged users are originating from
    Function: Logs
    Comments:
      - 'PowerShell Module: `Microsoft.PowerShell.Diagnostics`'
    MitreAttack:
  - Command: 'Get-WinEvent -ComputerName DC1.ad.bitsadmin.com -LogName ''Security'' -FilterXPath "*[System[(EventID=4768)]] and *[EventData[Data[@Name=''TargetUserName'']=''SomeAdmin'']]"'
    Description: Based on TGT request identify from which IP a user is authenticating
    Usecases:
      - Identify which IP a privileged user is originating from
    Function: Logs
    Comments:
      - 'PowerShell Module: `Microsoft.PowerShell.Diagnostics`'
    MitreAttack:
  - Command: 'Get-WinEvent -ComputerName W10.ad.bitsadmin.com -FilterHashtable @{logname="Security";id=4624} | % { [PSCustomObject]@{TimeCreated=$_.TimeCreated; SubjectUserSid=$_.Properties[0].Value; SubjectUserName=$_.Properties[1].Value; SubjectDomainName=$_.Properties[2].Value; SubjectLogonId=$_.Properties[3].Value; TargetUserSid=$_.Properties[4].Value; TargetUserName=$_.Properties[5].Value; TargetDomainName=$_.Properties[6].Value; TargetLogonId=$_.Properties[7].Value; LogonType=$_.Properties[8].Value; LogonProcessName=$_.Properties[9].Value; AuthenticationPackageName=$_.Properties[10].Value; WorkstationName=$_.Properties[11].Value; LogonGuid=$_.Properties[12].Value; TransmittedServices=$_.Properties[13].Value; LmPackageName=$_.Properties[14].Value; KeyLength=$_.Properties[15].Value; ProcessId=$_.Properties[16].Value; ProcessName=$_.Properties[17].Value; IpAddress=$_.Properties[18].Value; IpPort=$_.Properties[19].Value; ImpersonationLevel=$_.Properties[20].Value; RestrictedAdminMode=$_.Properties[21].Value; TargetOutboundUserName=$_.Properties[22].Value; TargetOutboundDomainName=$_.Properties[23].Value; VirtualAccount=$_.Properties[24].Value; TargetLinkedLogonId=$_.Properties[25].Value; ElevatedToken=$_.Properties[26].Value;} }'
    Description: List logons on a system
    Usecases:
      - Understand which accounts are used on a system
    Function: Logs
    Comments:
      - 'PowerShell Module: `Microsoft.PowerShell.Diagnostics`'
    MitreAttack:
  - Command: 'Get-WinEvent -ListLog * -ComputerName DC1.ad.bitsadmin.com'
    Description: Check which logs are enabled by viewing the number of records per log
    Usecases:
    Function: Logs
    Comments:
      - 'PowerShell Module: `Microsoft.PowerShell.Diagnostics`'
    MitreAttack:
Resources:
Detections:
Contributors:
    - Name: Arris Huijgen
      Handle: bitsadmin
---
