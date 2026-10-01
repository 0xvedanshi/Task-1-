# Task 1 — Foundation & Environment Setup

## Objective
Build core cybersecurity fundamentals and set up a working hacking lab for 
hands-on practice throughout the internship.

## Lab Environment
- **Hypervisor**: VirtualBox
- **Attacker machine**: Kali Linux
- **Target machine**: Metasploitable2
- **Network mode**: Host-Only Adapter, so both VMs sit on a private isolated subnet

## 1. Cybersecurity Basics
Covered the CIA Triad (Confidentiality, Integrity, Availability), common threat 
types (phishing, malware, DDoS, SQL injection, brute force, ransomware), and 
attack vectors (social engineering, wireless attacks, insider threats).

## 2. Lab Setup
Installed VirtualBox, configured Kali Linux as the attacker VM and Metasploitable2 
as the target VM, and set both to a Host-Only network so they can reach each other 
without exposing the lab to the internet.

**Screenshots:** `/screenshots/setup`
- `screenshots/setup/VirtualBox_kali_01_terminal.png` — Kali Linux booted and ready
- `screenshots/setup/VirtualBox_kali_ifconfig.png` / `screenshots/setup/VirtualBox_Metaspoitable2_ifconfig.png ` — confirming both VMs are on the same subnet
- `screenshots/setup/VirtualBox_kali_ping_targetVM.png` — verifying connectivity between attacker and target

## 3. Linux Fundamentals
Practiced file system navigation (`cd`, `ls`, `pwd`), permissions (`chmod`, `chown`), 
package management (`apt`, `dpkg`), and networking commands (`ifconfig`, `ping`, 
`netstat`, `traceroute`).

## 4. Networking Basics
Reviewed the OSI model layers, TCP/IP protocol suite, DNS/HTTP(S), and IP 
addressing/subnetting/NAT concepts that underpin the scanning work in Task 2.

## 5. Cryptography Basics
Covered symmetric vs asymmetric encryption and hashing (MD5, SHA256), then did a 
hands-on encrypt/decrypt exercise using OpenSSL.

**Screenshot:** `/screenshots/tools/VirtualBox_cryptotask1(1).png`

## 6. Tool Familiarization
- **Nmap** — ran a scan against the Metasploitable2 target → `screenshots/tools/VirtualBox_nmaptargetscan.png`
- **Wireshark** — captured ICMP traffic and inspected IP-level packet data → 
  `screenshots/tools/VirtualBox_wireshark_icmp.png`, `screenshots/tools/VirtualBox_wireshark_ipaddress.png`
- **Burp Suite** — set up the proxy and explored intercept/HTTP history → 
  `screenshots/tools/VirtualBox_burpsuite1.png`
- **Netcat** — tested file transfer between the two VMs → 
  `screenshots/tools/VirtualBox_netcat_filetransfer.png`

## Conclusion
The lab environment is fully functional, with Kali Linux and Metasploitable2 
communicating over an isolated host-only network. Core tooling (Nmap, Wireshark, 
Burp Suite, Netcat, OpenSSL) is installed and verified working, setting up the 
environment needed for Task 2's scanning and reconnaissance work.
