# ⚗️ ESXi-Home-SOC-Lab-Network-Overview 🧪
ESXi Home SOC Lab/Mock Network Overview

## Introduction/Goals

This project showcases my Home ESXi mock enterprise network and SOC Lab built on physical servers. The goal is to practice Network Engineering, Administration, Cybersecurity, and Ethical Hacking/Penetration Testing all in one lab. This is as on-going project that will be long term as in the future I will build, experiment, attack, and defend assets in a mock enterprise network that uses internet connectivity.

At a high level overview, here is what I have currently built: 

**Mock Enterprise Network**
- Windows Server 2019 Active Directory Server hosting ARK.local domain
- 2 Windows 10 Workstations under the ARK.local domain
- 1 Router outbound for internet access
- 1 Router configured with NAT, 3 interfaces for 3 Networks
- 1 Managed Switch with a SPAN/Mirror Port
  
**Security/SOC Tools:**
- Out of Band Security Onion instance passively collecting network traffic from the SPAN/Mirror port 

**Ethical Hacking/Penetration Testing Tools:**
- Kali Linux which sits internal to the 192.168.0.0/24 network, but is currently not joined to the domain.

## July 7 2023 Build 

![V2-01222021-CYBER-INTERFACE-HD](https://github.com/gervguerrero/ESXi-Home-SOC-Lab-Network-Overview/assets/140366635/f8ac453a-692e-44a9-9a44-2fef4073d9ac)


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
  
### Administration
- Joined 2 Windows 10 Pro workstations to ARK.local domain
- Created Users and set user privilege Group Policy Object (GPO) rules for 8 Users
  
### Cybersecurity
- Ingested and Analyzed network traffic for LLMNR/NBT-NS Poisoning Attack

### Ethical Hacking/Penetration Testing 
- Conducted internal LLMNR/NBT-NS Poisoning Attack to workstation in ARK.local domain
