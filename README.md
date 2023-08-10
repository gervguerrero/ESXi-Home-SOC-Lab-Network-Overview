# ⚗️ ESXi-Home-SOC-Lab-Network-Overview 🧪
ESXi Home SOC Lab/Mock Network Overview

## Introduction/Goals

This project showcases my Home ESXi mock enterprise network and SOC Lab built on physical servers. The goal is to practice Network Engineering, Administration, Cybersecurity, and Ethical Hacking/Penetration Testing all in one lab. This is an on-going project that will be long term as in the future I will build, experiment, attack, and defend assets in a mock enterprise network that uses internet connectivity.

At a high level overview, here is what I currently have built: 

**Mock Enterprise Network**
- Windows Server 2019 Active Directory Server hosting ARK.local domain
- 2 Windows 10 Workstations under the ARK.local domain
- 1 Router outbound for internet access
- 1 Router configured with NAT, 3 interfaces for 3 Networks
- 1 Managed Switch with a SPAN/Mirror Port
  
**Security/SOC Tools:**
- Out of Band Security Onion instance passively collecting network traffic from the SPAN/Mirror port 

**Ethical Hacking/Penetration Testing Tools:**
- Kali Linux which sits internal to the 192.168.10.0/24 network, but is currently not joined to the domain.

## July 7 2023 Build 

![V2-01222021-CYBER-INTERFACE-HD](https://github.com/gervguerrero/ESXi-Home-SOC-Lab-Network-Overview/assets/140366635/f006a8bb-ebc6-475c-be7a-9306522348ce)




## Overall Accomplishments:

### Network Engineering
- Set RAID 5 to both Physical Servers hosting ESXi
- Configured 2 ESXi servers
- Configured 1 Windows 2019 Active Directory Server
- Configured 2 Windows 10 Pro workstations
- Configured 1 Cisco Server with NAT and 3 Interfaces
- Configured Managed Switch with SPAN/Mirror Port
- Configured internal and internet connectivity in network
- Configured Security Onion to ingest from physical SPAN/Mirror Port
- Configured Kali Linux internal to mock network with internet connectivity
- Configured 1 Ubuntu Desktop Virtual Machine with internet connectivity in 192.168.0.0/24 Server space
  
### Administration
- Joined 2 Windows 10 Pro workstations to ARK.local domain
- Created users and set user privilege Group Policy Object (GPO) rules for 8 Users
- Applied GPO rules for User preference and display settings
- Installed Greenbone/OpenVAS on Kali Linux (Had some APT update errors in the process)
- Converted Ubuntu Desktop to Server and installed MySQL application through CLI. 
  
### Cybersecurity
- Ingested and Analyzed network traffic for LLMNR/NBT-NS Poisoning Attack (Link Local Multi Namecast Resolution / Netbios Name Service Poisoning)

### Ethical Hacking/Penetration Testing 
- Conducted internal LLMNR/NBT-NS Poisoning Attack to workstation in ARK.local domain (Link Local Multi Namecast Resolution / Netbios Name Service Poisoning)


## Future Goals:

### Network Engineering
- Create an Vulnerable Ubuntu Web Server on the Network
- Add 1 or 2 more Windows 10 Pro Workstations
- Installing PFsense Firewall 
- Creating a SQL Database server
  
### Administration
- Set GPO rules to baseline workstations with default authorized software
- Set GPO rules to block and detect installing unauthorized software
- Set GPO rules to block and detect unauthorized USB storage device usage
- Set GPO rules to block and detect requests to unauthorized websites

  
### Cybersecurity
- Installing PFsense Firewall
- Creating a Velociraptor Endpoint Detection & Response Server
- Ingesting Windows Event Logs into Security Onion SIEM
- Deploying Sysmon Logging on network assets
- Ingesting Sysmon Logs into Security Onion SIEM
- Creating/Testing Temporary Splunk Server as another SIEM
- Test custom Suricata/Yara Rules in Security Onion 
- Create a Malware Analysis Server
- Detect and Analyze attacks launched from Kali VM
  
### Ethical Hacking/Penetration Testing 
- Nmap scan network
- Exploit vulnerable assets on network
- Launch Ransomware on Windows workstation
- Perform keberoasting/SMB relaying on network
- Create backdoor persistence in Registry Keys
- Create fake website hosting malicious scripts
- Create Phishing Email with payload in attachments
- Use a Redirector to perform malicious actions
- Launch a Keylogger on Windows workstation
- Perform SSL Stripping Attack 
