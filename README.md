# ⚗️ ESXi-Home-SOC-Lab-Network-Overview 🧪
ESXi Home SOC Lab/Mock Network Overview

## Introduction/Goals

This project showcases my Home ESXi mock enterprise network and SOC Lab built on physical servers. The goal is to practice Network Engineering, Administration, Cybersecurity, and Ethical Hacking/Penetration Testing all in one lab. This is as on-going project that will be long term as in the future I will build, experiment, attack, and defend assets in a mock enterprise network that uses internet connectivity.

At a high level overview, I have built a small Active Directory Domain with 2 Windows 10 machines and 1 Domain Controller. Using a physical switch, I set up a SPAN/Mirror port to replicate and monitor traffic which is ingested into my Security Onion instance for analysis. The Kali VM I have currently acts as an attacker that sits internal to the ARK.local domain in the 192.168.0.0/24 network, but is currently not joined to the domain. 

# July 7 2023 Build 

![V2-01222021-CYBER-INTERFACE-HD](https://github.com/gervguerrero/ESXi-Home-SOC-Lab-Network-Overview/assets/140366635/f8ac453a-692e-44a9-9a44-2fef4073d9ac)
