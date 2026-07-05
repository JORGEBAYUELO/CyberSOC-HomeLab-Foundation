# CyberSOC HomeLab Foundation

![HeroBanner](/images/GitHub-HomeLab-Foundation-Banner.jpg)

> Building a production inspired cybersecurity home lab focused on blue team operations, detection engineering, threat hunting, incident response, and security automation.

---

## Project Overview

The CyberSOC HomeLab Foundation repository documents the infrastructure used throughout my cybersecurity portfolio.

Rather than deploying isolated tools, this project focuses on building a realistic enterprise inspired environment that can be expanded into multiple security disciplines including:

- Security Operations Center (SOC)
- Detection Engineering
- Threat Hunting
- Incident Response
- Active Directory Security
- Purple Teaming
- Malware Analysis
- Security Automation

This repository serves as the baseline infrastructure for all future CyberSOC projects.

---

## Objectives

The primary goals of this project are:

- Build an enterprise inspired Active Directory environment
- Deploy centralized DNS services
- Configure a segmented virtual network
- Deploy a SIEM platform using Wazuh
- Create Windows and Linux endpoints
- Build an attacker workstation using Kali Linux
- Validate enterprise network communications
- Create reusable infrastructure for future detection engineering projects

---

## Lab Architecture

![Architecture Diagram](/images/Foundational-Architectural-Diagram.jpg)

---

## Technologies

| Category | Technology |
|----------|------------|
| Hypervisor | VMware Workstation Pro |
| Directory Services | Windows Server 2022 |
| Identity | Active Directory |
| DNS | Microsoft DNS |
| SIEM | Wazuh |
| Endpoint | Windows 11 Enterprise |
| Offensive Security | Kali Linux |
| Remote Access | OpenSSH |
| Networking | VMware VMnet2 |

---

## Virtual Machines

| Machine | Role | IP Address |
|----------|------|------------|
| Cyber-DC01 | Domain Controller / DNS | 192.168.100.10 |
| WIN11-CLIENT01 | Enterprise Workstation | 192.168.100.20 |
| Wazuh-Server01 | SIEM Platform | 192.168.100.30 |
| Kali-Attacker01 | Offensive Security Workstation | 192.168.100.40 |

---

## Network Design

Domain:

```
cybersoc.lab
```

Subnet:

```
192.168.100.0/24
```

DNS Server:

```
192.168.100.10
```

Reverse Lookup Zone:

```
100.168.192.in-addr.arpa
```

---

## VMware infrastructure

- Cyber-DC01

![Cyber-DC01](/images/)

- WIN11-CLIENT01

![WIN11-CLIENT01](/images/)

- Wazuh-Server01

![Wazuh-Server01](/images/)

- Kali-Attacker01

![Kali-Attacker01](/images/)

---

## Active Directory

---

## DNS

---

## Wazuh

---

## Networking

---

## Remote Administration

---

## Features Completed

- Active Directory deployment
- Domain configuration
- DNS Forward Lookup Zone
- DNS Reverse Lookup Zone
- Static IP addressing
- Hostname resolution
- Forward DNS resolution
- Reverse DNS resolution
- Wazuh deployment
- Kali Linux deployment
- SSH configuration
- Network validation
- Cross-platform connectivity testing

---

## Validation

The following functionality has been successfully verified.

| Validation | Status |
|------------|--------|
| Active Directory | Complete |
| DNS Forward Resolution | Complete |
| Reverse DNS Resolution | Complete |
| ICMP Connectivity | Complete |
| SSH Access | Complete |
| Wazuh Dashboard | Complete |
| Static IP Configuration | Complete |

---

## Roadmap

Upcoming projects built on top of this foundation include:

- Detection Engineering
- Sysmon Deployment
- Windows Event Forwarding
- Sigma Rules
- MITRE ATT&CK Mapping
- Threat Hunting
- Incident Response
- Active Directory Attacks
- Purple Team Exercises
- Security Automation
- SOAR Integrations

---

## Lessons Learned

Throughout the build process I encountered and resolved several real-world infrastructure issues including:

- DNS forward lookup troubleshooting
- Reverse lookup zone configuration
- PTR record creation
- Hostname resolution failures
- Static IP configuration in Linux
- SSH service troubleshooting
- Cross-platform DNS validation

These troubleshooting exercises provided practical experience with enterprise networking and systems administration concepts commonly encountered in SOC and infrastructure environments.

---

## License

This project is licensed under the MIT License.

---

## Author

**Jorge Bayuelo**

Cybersecurity Analyst

CompTIA Security+

CompTIA CySA+

Building practical cybersecurity projects focused on blue team operations, detection engineering, and enterprise security.
