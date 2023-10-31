# Turla - G0010

**Created**: 2017-05-31T21:31:49.816Z

**Modified**: 2023-03-22T05:41:28.428Z

**Contributors**: Matthieu Faou, ESET,Edward Millington

## Aliases

Turla,IRON HUNTER,Group 88,Belugasturgeon,Waterbug,WhiteBear,Snake,Krypton,Venomous Bear

## Description

[Turla](https://attack.mitre.org/groups/G0010) is a Russian-based threat group that has infected victims in over 45 countries, spanning a range of industries including government, embassies, military, education, research and pharmaceutical companies since 2004. Heightened activity was seen in mid-2015. [Turla](https://attack.mitre.org/groups/G0010) is known for conducting watering hole and spearphishing campaigns and leveraging in-house tools and malware. [Turla](https://attack.mitre.org/groups/G0010)’s espionage platform is mainly used against Windows machines, but has also been seen used against macOS and Linux machines.(Citation: Kaspersky Turla)(Citation: ESET Gazer Aug 2017)(Citation: CrowdStrike VENOMOUS BEAR)(Citation: ESET Turla Mosquito Jan 2018)

## Techniques Used

|Matrix|Domain|Platform|Technique ID|Technique Name|Use|
| :---| :---| :---| :---| :---| :---|
|mitre-attack|enterprise-attack|Windows|T1112|Modify Registry|[Turla](https://attack.mitre.org/groups/G0010) has modify Registry values to store payloads.(Citation: ESET Turla PowerShell May 2019)(Citation: Symantec Waterbug Jun 2019)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1090.001|Internal Proxy|[Turla](https://attack.mitre.org/groups/G0010) has compromised internal network systems to act as a proxy to forward traffic to C2.(Citation: Talos TinyTurla September 2021)|
|mitre-attack|enterprise-attack|Windows|T1615|Group Policy Discovery|[Turla](https://attack.mitre.org/groups/G0010) surveys a system upon check-in to discover Group Policy details using the <code>gpresult</code> command.(Citation: ESET ComRAT May 2020)|
|mitre-attack|enterprise-attack|PRE|T1588.002|Tool|[Turla](https://attack.mitre.org/groups/G0010) has obtained and customized publicly-available tools like [Mimikatz](https://attack.mitre.org/software/S0002).(Citation: Symantec Waterbug Jun 2019)|
|mitre-attack|enterprise-attack|Windows,macOS,Linux|T1059.007|JavaScript|[Turla](https://attack.mitre.org/groups/G0010) has used various JavaScript-based backdoors.(Citation: ESET Turla Mosquito Jan 2018)	|
|mitre-attack|enterprise-attack|Windows,macOS|T1553.006|Code Signing Policy Modification|[Turla](https://attack.mitre.org/groups/G0010) has modified variables in kernel memory to turn off Driver Signature Enforcement after exploiting vulnerabilities that obtained kernel mode privileges.(Citation: Unit42 AcidBox June 2020)(Citation: GitHub Turla Driver Loader)|
|mitre-attack|enterprise-attack|Windows,Linux,macOS|T1016.001|Internet Connection Discovery|[Turla](https://attack.mitre.org/groups/G0010) has used <code>tracert</code> to check internet connectivity.(Citation: ESET ComRAT May 2020)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows,Containers|T1068|Exploitation for Privilege Escalation|[Turla](https://attack.mitre.org/groups/G0010) has exploited vulnerabilities in the VBoxDrv.sys driver to obtain kernel mode privileges.(Citation: Unit42 AcidBox June 2020)|
|mitre-attack|enterprise-attack|Linux,Windows,macOS|T1059.006|Python|[Turla](https://attack.mitre.org/groups/G0010) has used IronPython scripts as part of the [IronNetInjector](https://attack.mitre.org/software/S0581) toolchain to drop payloads.(Citation: Unit 42 IronNetInjector February 2021 )|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1071.003|Mail Protocols|[Turla](https://attack.mitre.org/groups/G0010) has used multiple backdoors which communicate with a C2 server via email attachments.(Citation: Crowdstrike GTR2020 Mar 2020)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows,Containers|T1078.003|Local Accounts|[Turla](https://attack.mitre.org/groups/G0010) has abused local accounts that have the same password across the victim’s network.(Citation: ESET Crutch December 2020)|
|mitre-attack|enterprise-attack|PRE|T1583.006|Web Services|[Turla](https://attack.mitre.org/groups/G0010) has created web accounts including Dropbox and GitHub for C2 and document exfiltration.(Citation: ESET Crutch December 2020)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1102|Web Service|[Turla](https://attack.mitre.org/groups/G0010) has used legitimate web services including Pastebin, Dropbox, and GitHub for C2 communications.(Citation: Accenture HyperStack October 2020)(Citation: ESET Crutch December 2020)|
|mitre-attack|enterprise-attack|PRE|T1587.001|Malware|[Turla](https://attack.mitre.org/groups/G0010) has developed its own unique malware for use in operations.(Citation: Recorded Future Turla Infra 2020)|
|mitre-attack|enterprise-attack|PRE|T1584.004|Server|[Turla](https://attack.mitre.org/groups/G0010) has used compromised servers as infrastructure.(Citation: Recorded Future Turla Infra 2020)(Citation: Accenture HyperStack October 2020)(Citation: Talos TinyTurla September 2021)|
|mitre-attack|enterprise-attack|PRE|T1584.006|Web Services|[Turla](https://attack.mitre.org/groups/G0010) has frequently used compromised WordPress sites for C2 infrastructure.(Citation: Recorded Future Turla Infra 2020)|
|mitre-attack|enterprise-attack|PRE|T1584.003|Virtual Private Server|[Turla](https://attack.mitre.org/groups/G0010) has used the VPS infrastructure of compromised Iranian threat actors.(Citation: NSA NCSC Turla OilRig)|
|mitre-attack|enterprise-attack|PRE|T1588.001|Malware|[Turla](https://attack.mitre.org/groups/G0010) has used malware obtained after compromising other threat actors, such as [OilRig](https://attack.mitre.org/groups/G0049).(Citation: NSA NCSC Turla OilRig)(Citation: Recorded Future Turla Infra 2020)|
|mitre-attack|enterprise-attack|Windows,Azure AD,Office 365,SaaS,IaaS,Linux,macOS,Google Workspace|T1518.001|Security Software Discovery|[Turla](https://attack.mitre.org/groups/G0010) has obtained information on security software, including security logging information that may indicate whether their malware has been detected.(Citation: ESET ComRAT May 2020)|
|mitre-attack|enterprise-attack|Windows,Linux,macOS,SaaS|T1189|Drive-by Compromise|[Turla](https://attack.mitre.org/groups/G0010) has infected victims using watering holes.(Citation: ESET ComRAT May 2020)(Citation: Secureworks IRON HUNTER Profile)|
|mitre-attack|enterprise-attack|Linux,Windows,macOS,SaaS,Office 365,Google Workspace,IaaS|T1213|Data from Information Repositories|[Turla](https://attack.mitre.org/groups/G0010) has used a custom .NET tool to collect documents from an organization's internal central database.(Citation: ESET ComRAT May 2020)|
|mitre-attack|enterprise-attack|Windows,macOS,Linux|T1120|Peripheral Device Discovery|[Turla](https://attack.mitre.org/groups/G0010) has used <code>fsutil fsinfo drives</code> to list connected drives.(Citation: ESET ComRAT May 2020)|
|mitre-attack|enterprise-attack|Windows,Linux,macOS,IaaS,Network|T1201|Password Policy Discovery|[Turla](https://attack.mitre.org/groups/G0010) has used <code>net accounts</code> and <code>net accounts /domain</code> to acquire password policy information.(Citation: ESET ComRAT May 2020)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1087.001|Local Account|[Turla](https://attack.mitre.org/groups/G0010) has used <code>net user</code> to enumerate local accounts on the system.(Citation: ESET ComRAT May 2020)(Citation: ESET Crutch December 2020)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1087.002|Domain Account|[Turla](https://attack.mitre.org/groups/G0010) has used <code>net user /domain</code> to enumerate domain accounts.(Citation: ESET ComRAT May 2020)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1069.001|Local Groups|[Turla](https://attack.mitre.org/groups/G0010) has used <code>net localgroup</code> and <code>net localgroup Administrators</code> to enumerate group information, including members of the local administrators group.(Citation: ESET ComRAT May 2020)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1069.002|Domain Groups|[Turla](https://attack.mitre.org/groups/G0010) has used <code>net group "Domain Admins" /domain</code> to identify domain administrators.(Citation: ESET ComRAT May 2020)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1570|Lateral Tool Transfer|[Turla](https://attack.mitre.org/groups/G0010) RPC backdoors can be used to transfer files to/from victim machines on the local network.(Citation: ESET Turla PowerShell May 2019)(Citation: Symantec Waterbug Jun 2019)|
|mitre-attack|enterprise-attack|Windows|T1055.001|Dynamic-link Library Injection|[Turla](https://attack.mitre.org/groups/G0010) has used Metasploit to perform reflective DLL injection in order to escalate privileges.(Citation: ESET Turla Mosquito May 2018)(Citation: Github Rapid7 Meterpreter Elevate)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1560.001|Archive via Utility|[Turla](https://attack.mitre.org/groups/G0010) has encrypted files stolen from connected USB drives into a RAR file before exfiltration.(Citation: Symantec Waterbug Jun 2019)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1567.002|Exfiltration to Cloud Storage|[Turla](https://attack.mitre.org/groups/G0010) has used WebDAV to upload stolen USB files to a cloud drive.(Citation: Symantec Waterbug Jun 2019) [Turla](https://attack.mitre.org/groups/G0010) has also exfiltrated stolen files to OneDrive and 4shared.(Citation: ESET ComRAT May 2020)|
|mitre-attack|enterprise-attack|Windows,macOS,Linux|T1059.005|Visual Basic|[Turla](https://attack.mitre.org/groups/G0010) has used VBS scripts throughout its operations.(Citation: Symantec Waterbug Jun 2019)	|
|mitre-attack|enterprise-attack|Windows|T1555.004|Windows Credential Manager|[Turla](https://attack.mitre.org/groups/G0010) has gathered credentials from the Windows Credential Manager tool.(Citation: Symantec Waterbug Jun 2019)	|
|mitre-attack|enterprise-attack|Windows|T1059.003|Windows Command Shell|[Turla](https://attack.mitre.org/groups/G0010) RPC backdoors have used cmd.exe to execute commands.(Citation: ESET Turla PowerShell May 2019)(Citation: Symantec Waterbug Jun 2019)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows,Network|T1005|Data from Local System|[Turla](https://attack.mitre.org/groups/G0010) RPC backdoors can upload files from victim machines.(Citation: ESET Turla PowerShell May 2019)|
|mitre-attack|enterprise-attack|Windows|T1134.002|Create Process with Token|[Turla](https://attack.mitre.org/groups/G0010) RPC backdoors can impersonate or steal process tokens before executing commands.(Citation: ESET Turla PowerShell May 2019)	|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1025|Data from Removable Media|[Turla](https://attack.mitre.org/groups/G0010) RPC backdoors can collect files from USB thumb drives.(Citation: ESET Turla PowerShell May 2019)(Citation: Symantec Waterbug Jun 2019)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows,Network|T1090|Proxy|[Turla](https://attack.mitre.org/groups/G0010) RPC backdoors have included local UPnP RPC proxies.(Citation: ESET Turla PowerShell May 2019)	|
|mitre-attack|enterprise-attack|Windows,Linux,macOS|T1140|Deobfuscate/Decode Files or Information|[Turla](https://attack.mitre.org/groups/G0010) has used a custom decryption routine, which pulls key and salt values from other artifacts such as a WMI filter or [PowerShell Profile](https://attack.mitre.org/techniques/T1546/013), to decode encrypted PowerShell payloads.(Citation: ESET Turla PowerShell May 2019)|
|mitre-attack|enterprise-attack|Windows,macOS,Linux,Containers,IaaS|T1562.001|Disable or Modify Tools|[Turla](https://attack.mitre.org/groups/G0010) has used a AMSI bypass, which patches the in-memory amsi.dll, in PowerShell scripts to bypass Windows antimalware products.(Citation: ESET Turla PowerShell May 2019)|
|mitre-attack|enterprise-attack|Windows,macOS,Linux|T1106|Native API|[Turla](https://attack.mitre.org/groups/G0010) and its RPC backdoors have used APIs calls for various tasks related to subverting AMSI and accessing then executing commands through RPC and/or named pipes.(Citation: ESET Turla PowerShell May 2019)|
|mitre-attack|enterprise-attack|Windows|T1546.003|Windows Management Instrumentation Event Subscription|[Turla](https://attack.mitre.org/groups/G0010) has used WMI event filters and consumers to establish persistence.(Citation: ESET Turla PowerShell May 2019)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1027.010|Command Obfuscation|[Turla](https://attack.mitre.org/groups/G0010) has used encryption (including salted 3DES via [PowerSploit](https://attack.mitre.org/software/S0194)'s <code>Out-EncryptedScript.ps1</code>), random variable names, and base64 encoding to obfuscate PowerShell commands and payloads.(Citation: ESET Turla PowerShell May 2019)|
|mitre-attack|enterprise-attack|Windows|T1027.011|Fileless Storage|[Turla](https://attack.mitre.org/groups/G0010) has used the Registry to store encrypted and encoded payloads.(Citation: ESET Turla PowerShell May 2019)(Citation: Symantec Waterbug Jun 2019)|
|mitre-attack|enterprise-attack|Windows|T1546.013|PowerShell Profile|[Turla](https://attack.mitre.org/groups/G0010) has used PowerShell profiles to maintain persistence on an infected machine.(Citation: ESET Turla PowerShell May 2019)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows,Office 365,SaaS,Google Workspace|T1566.002|Spearphishing Link|[Turla](https://attack.mitre.org/groups/G0010) attempted to trick targets into clicking on a link featuring a seemingly legitimate domain from Adobe.com to download their malware and gain initial access.(Citation: ESET Turla Mosquito Jan 2018)|
|mitre-attack|enterprise-attack|Windows|T1547.001|Registry Run Keys / Startup Folder|A [Turla](https://attack.mitre.org/groups/G0010) Javascript backdoor added a local_update_check value under the Registry key <code>HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\Run</code> to establish persistence. Additionally, a [Turla](https://attack.mitre.org/groups/G0010) custom executable containing Metasploit shellcode is saved to the Startup folder to gain persistence.(Citation: ESET Turla Mosquito Jan 2018)(Citation: ESET Turla Mosquito May 2018)|
|mitre-attack|enterprise-attack|Windows|T1059.001|PowerShell|[Turla](https://attack.mitre.org/groups/G0010) has used PowerShell to execute commands/scripts, in some cases via a custom executable or code from [Empire](https://attack.mitre.org/software/S0363)'s PSInject.(Citation: ESET Turla Mosquito May 2018)(Citation: ESET Turla PowerShell May 2019)(Citation: Symantec Waterbug Jun 2019) [Turla](https://attack.mitre.org/groups/G0010) has also used PowerShell scripts to load and execute malware in memory.|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1071.001|Web Protocols|[Turla](https://attack.mitre.org/groups/G0010) has used HTTP and HTTPS for C2 communications.(Citation: ESET Turla Mosquito Jan 2018)(Citation: ESET Turla Mosquito May 2018)|
|mitre-attack|enterprise-attack|Windows|T1547.004|Winlogon Helper DLL|[Turla](https://attack.mitre.org/groups/G0010) established persistence by adding a Shell value under the Registry key <code>HKCU\Software\Microsoft\Windows NT\CurrentVersion\Winlogon</code>.(Citation: ESET Turla Mosquito Jan 2018)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1105|Ingress Tool Transfer|[Turla](https://attack.mitre.org/groups/G0010) has used shellcode to download Meterpreter after compromising a victim.(Citation: ESET Turla Mosquito May 2018)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1102.002|Bidirectional Communication|A [Turla](https://attack.mitre.org/groups/G0010) JavaScript backdoor has used Google Apps Script as its C2 server.(Citation: ESET Turla Mosquito Jan 2018)(Citation: ESET Turla Mosquito May 2018)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1055|Process Injection|[Turla](https://attack.mitre.org/groups/G0010) has also used [PowerSploit](https://attack.mitre.org/software/S0194)'s <code>Invoke-ReflectivePEInjection.ps1</code> to reflectively load a PowerShell payload into a random process on the victim system.(Citation: ESET Turla PowerShell May 2019)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1204.001|Malicious Link|[Turla](https://attack.mitre.org/groups/G0010) has used spearphishing via a link to get users to download and run their malware.(Citation: ESET Turla Mosquito Jan 2018)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows|T1027.005|Indicator Removal from Tools|Based on comparison of [Gazer](https://attack.mitre.org/software/S0168) versions, [Turla](https://attack.mitre.org/groups/G0010) made an effort to obfuscate strings in the malware that could be used as IoCs, including the mutex name and named pipe.(Citation: ESET Gazer Aug 2017)|
|mitre-attack|enterprise-attack|Windows,Network|T1124|System Time Discovery|[Turla](https://attack.mitre.org/groups/G0010) surveys a system upon check-in to discover the system time by using the <code>net time</code> command.(Citation: Kaspersky Turla)|
|mitre-attack|enterprise-attack|Windows|T1021.002|SMB/Windows Admin Shares|[Turla](https://attack.mitre.org/groups/G0010) used <code>net use</code> commands to connect to lateral systems within a network.(Citation: Kaspersky Turla)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows,Network|T1083|File and Directory Discovery|[Turla](https://attack.mitre.org/groups/G0010) surveys a system upon check-in to discover files in specific locations on the hard disk %TEMP% directory, the current user's desktop, the Program Files directory, and Recent.(Citation: Kaspersky Turla)(Citation: ESET ComRAT May 2020) [Turla](https://attack.mitre.org/groups/G0010) RPC backdoors have also searched for files matching the <code>lPH*.dll</code> pattern.(Citation: ESET Turla PowerShell May 2019)|
|mitre-attack|enterprise-attack|Windows,IaaS,Linux,macOS,Network|T1082|System Information Discovery|[Turla](https://attack.mitre.org/groups/G0010) surveys a system upon check-in to discover operating system configuration details using the <code>systeminfo</code> and <code>set</code> commands.(Citation: Kaspersky Turla)(Citation: ESET ComRAT May 2020)|
|mitre-attack|enterprise-attack|Windows,Azure AD,Office 365,SaaS,IaaS,Linux,macOS,Google Workspace,Containers,Network|T1110|Brute Force|[Turla](https://attack.mitre.org/groups/G0010) may attempt to connect to systems within a victim's network using <code>net use</code> commands and a predefined list or collection of passwords.(Citation: Kaspersky Turla)|
|mitre-attack|enterprise-attack|Windows,IaaS,Linux,macOS,Network|T1049|System Network Connections Discovery|[Turla](https://attack.mitre.org/groups/G0010) surveys a system upon check-in to discover active local network connections using the <code>netstat -an</code>, <code>net use</code>, <code>net file</code>, and <code>net session</code> commands.(Citation: Kaspersky Turla)(Citation: ESET ComRAT May 2020) [Turla](https://attack.mitre.org/groups/G0010) RPC backdoors have also enumerated the IPv4 TCP connection table via the <code>GetTcpTable2</code> API call.(Citation: ESET Turla PowerShell May 2019)|
|mitre-attack|enterprise-attack|Windows|T1012|Query Registry|[Turla](https://attack.mitre.org/groups/G0010) surveys a system upon check-in to discover information in the Windows Registry with the <code>reg query</code> command.(Citation: Kaspersky Turla) [Turla](https://attack.mitre.org/groups/G0010) has also retrieved PowerShell payloads hidden in Registry keys as well as checking keys associated with null session named pipes .(Citation: ESET Turla PowerShell May 2019)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows,Network|T1018|Remote System Discovery|[Turla](https://attack.mitre.org/groups/G0010) surveys a system upon check-in to discover remote systems on a local network using the <code>net view</code> and <code>net view /DOMAIN</code> commands. [Turla](https://attack.mitre.org/groups/G0010) has also used <code>net group "Domain Computers" /domain</code>, <code>net group "Domain Controllers" /domain</code>, and <code>net group "Exchange Servers" /domain</code> to enumerate domain computers, including the organization's DC and Exchange Server.(Citation: Kaspersky Turla)(Citation: ESET ComRAT May 2020)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows,Network|T1016|System Network Configuration Discovery|[Turla](https://attack.mitre.org/groups/G0010) surveys a system upon check-in to discover network configuration details using the <code>arp -a</code>, <code>nbtstat -n</code>, <code>net config</code>, <code>ipconfig /all</code>, and <code>route</code> commands, as well as [NBTscan](https://attack.mitre.org/software/S0590).(Citation: Kaspersky Turla)(Citation: Symantec Waterbug Jun 2019)(Citation: ESET ComRAT May 2020) [Turla](https://attack.mitre.org/groups/G0010) RPC backdoors have also retrieved registered RPC interface information from process memory.(Citation: ESET Turla PowerShell May 2019)|
|mitre-attack|enterprise-attack|Linux,macOS,Windows,Network|T1057|Process Discovery|[Turla](https://attack.mitre.org/groups/G0010) surveys a system upon check-in to discover running processes using the <code>tasklist /v</code> command.(Citation: Kaspersky Turla) [Turla](https://attack.mitre.org/groups/G0010) RPC backdoors have also enumerated processes associated with specific open ports or named pipes.(Citation: ESET Turla PowerShell May 2019)|
|mitre-attack|enterprise-attack|Windows,macOS,Linux|T1007|System Service Discovery|[Turla](https://attack.mitre.org/groups/G0010) surveys a system upon check-in to discover running services and associated processes using the <code>tasklist /svc</code> command.(Citation: Kaspersky Turla)|