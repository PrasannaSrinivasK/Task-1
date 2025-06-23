# Task 1: Scan Your Local Network for Open Ports

## Objective
Perform a basic port scan on a target system within the local network to understand network exposure and identify open services.

## Tools Used
- Nmap – For active network scanning  
- Wireshark – For optional packet analysis (used for verification and deeper insights)

## Steps Performed

1. Booted into Kali Linux for a secure and powerful penetration testing environment.
2. Identified the target IP address in the local network: `10.10.201.252`
3. Executed the following Nmap command in terminal:
   bash
   nmap -sS -sV -Pn -oN nmap.txt 10.10.201.252
-sS: TCP SYN scan
-sV: Service version detection
-Pn: Skip host discovery (treat target as up)
-oN: Save results to nmap.txt

Analyzed the scan results and noted down open ports and running services.
Opened Wireshark to observe and analyze packet-level traffic during scanning for learning purposes.
Saved all relevant screenshots in the main directory for documentation.

## Output Files:
nmap.txt – Raw Nmap scan results
screenshots/ – Visual evidence of the scanning and analysis process

## Observations:
Identified open ports and their associated services.
Verified scan behavior using Wireshark.
Learned how unauthorized open ports can pose a potential security risk in a network.

## Key Concepts Covered:
Port Scanning (TCP SYN Scan)
Service Enumeration
Network Reconnaissance
Local IP Range Targeting
Packet Analysis with Wireshark
Network Security Fundamentals

## Outcome:
Gained hands-on experience with basic network reconnaissance techniques and understood how to interpret scan results for potential vulnerabilities.
