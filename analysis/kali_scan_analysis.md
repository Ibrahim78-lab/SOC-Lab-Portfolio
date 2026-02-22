# Analysis: Kali Nmap Scan

## Overview
This analysis covers the alerts generated when Kali Linux performed an Nmap scan against the Wazuh Agent and Manager.

## Key Alerts Observed
- ET SCAN NMAP -sS scan
- PORT SCAN detected
- UDP SCAN detected

## Source and Destination
- Source: 192.168.1.23 (Kali)
- Destination: 192.168.1.5 (Agent 006)

## Interpretation
The alerts indicate:
- A SYN stealth scan (-sS)
- A UDP scan
- Multiple port probes

These are typical reconnaissance activities used by attackers to map open ports and services.

## Conclusion
Suricata successfully detected the malicious scanning activity, and the Manager received the alerts correctly.
