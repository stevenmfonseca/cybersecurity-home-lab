
# Cybersecurity Home Lab – Metasploitable Exploit

## Overview
This project demonstrates a penetration testing home lab built using VirtualBox.

An attacker machine running Kali Linux was used to scan and exploit a vulnerable
Metasploitable machine.

## Lab Environment

Attacker Machine:
- Kali Linux

Target Machine:
- Metasploitable 2

Virtualization:
- VirtualBox

## Network Diagram

Kali Linux (Attacker) 
        |
        |
Host-only network
        |
        |
      
Metasploitable (Target)

## Tools Used

- Nmap
- Metasploit Framework

## Steps Performed

### 1. Network Discovery
Identified target IP and verified connectivity using ping.

### 2. Port Scanning
Used Nmap to identify open ports and services including FTP, SSH, Telnet, and HTTP.

### 3. Vulnerability Identification
Discovered vulnerable vsftpd FTP service running on port 21.

### 4. Exploitation
Used Metasploit module:

exploit/unix/ftp/vsftpd_234_backdoor

### 5. Root Access
Successfully obtained root shell access on the target machine.

## Screenshots

See the /screenshots folder.
