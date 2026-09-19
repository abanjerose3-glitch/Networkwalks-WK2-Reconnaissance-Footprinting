# 🔎 Networkwalks — Week 2 Reconnaissance & Footprinting

<p align="center">

### 🛡️ Cybersecurity Internship Laboratory

**Footprinting • Reconnaissance • OSINT • Network Discovery**

</p>

---

## 📌 Project Overview

This repository documents my **Week 2 Cybersecurity Internship laboratory activities at Networkwalks**, focusing on reconnaissance, footprinting, open-source information gathering, and network discovery.

The activities demonstrate how cybersecurity professionals can gather information about an authorized target and analyze network visibility during the early stages of a security assessment.

The project covers:

- Domain footprinting
- DNS reconnaissance
- Web technology fingerprinting
- HTTP header analysis
- Web Application Firewall detection
- DNS enumeration
- Google-based reconnaissance
- OSINT techniques
- Network host discovery
- IP and MAC address identification
- Network topology visualization
- Cybersecurity evidence collection and documentation

---

# Objectives

The main objectives of this project were to:

- Understand the reconnaissance and footprinting phase of a security assessment.
- Learn how publicly available information can reveal details about an organization.
- Practice using multiple reconnaissance tools available in Kali Linux.
- Perform DNS and web reconnaissance.
- Understand basic OSINT techniques.
- Identify active hosts within an authorized local network.
- Identify IP and MAC addresses of discovered hosts.
- Visualize network topology using Zenmap.
- Document technical procedures and evidence professionally.
- Develop practical cybersecurity troubleshooting and reporting skills.

---

# Project Scope

## Authorized Targets / Environments

The activities were performed within the authorized educational environment provided for the Networkwalks Cybersecurity Internship.

### Reconnaissance Target

```text
networkwalks.com
Network Scanning Target
My authorized local/LAN network
```

Network scanning activities were limited to the authorized local environment used for the laboratory exercise.

# Tools & Technologies
Tool	Purpose
Kali Linux	Cybersecurity testing and reconnaissance environment
WHOIS	Domain registration and ownership-related information
WhatWeb	Web technology fingerprinting
NSLookup	DNS resolution and investigation
cURL	HTTP response header inspection
wafw00f	Web Application Firewall detection
DNSRecon	DNS enumeration
Google / GHDB	Search-based reconnaissance
Maltego	Visual reconnaissance and OSINT
theHarvester	Open-source information gathering
Zenmap	Graphical network scanning
Nmap	Network discovery and scanning engine
Windows CMD	Local IP and MAC address identification

# Week 2 Modules

| Module | Activity | Status |
|---|---|---|
| W2-PM1 | Footprinting with Multiple Kali Tools | ✅ Completed |
| W2-PM2 | Google Hacking Database | ✅ Completed |
| W2-PM4 | Footprinting with theHarvester | ✅ Completed |
| W2-PM5 | Network Scanning with Zenmap | ✅ Completed |

Module status reflects the laboratory work and evidence documented in this repository.

# W2-PM1 — Footprinting & Reconnaissance with Multiple Kali Tools
Overview

This laboratory exercise focused on performing footprinting and reconnaissance using multiple tools available in Kali Linux.

The activity uses six reconnaissance tools:

WHOIS
WhatWeb
NSLookup
cURL
wafw00f
DNSRecon

The purpose is to understand what information can be observed from publicly accessible services during the reconnaissance phase.

## WHOIS
Command
whois networkwalks.com
Purpose

WHOIS was used to retrieve publicly available domain registration and infrastructure-related information.

Evidence

📸 Screenshot:
evidence/PM1-WHOIS.png

Observation

The command returned publicly available domain-related information.

Actual observation:

Add the relevant information from my own command output here.

# WhatWeb
Command
whatweb networkwalks.com
Purpose

WhatWeb was used to identify technologies and web-related information exposed by the target.

Evidence

📸 Screenshot:
evidence/PM1-WhatWeb.png

Observation

The output identified technologies associated with the website.

Actual observation:

Add the technologies identified from my own output here.

# NSLookup
Command
nslookup networkwalks.com
Purpose

NSLookup was used to investigate DNS resolution information associated with the target domain.

Evidence

📸 Screenshot:
evidence/PM1-NSLookup.png

Observation

The command returned DNS resolution information.

Actual result:

Domain:
IP Address:
DNS Server:

Replace these fields with the actual values from my evidence.

# cURL — HTTP Header Analysis
Command
curl -I https://networkwalks.com
Purpose

cURL was used to inspect HTTP response headers returned by the web server.

Evidence

📸 Screenshot:
evidence/PM1-cURL.png

Observation

The HTTP response contained several server and security-related headers.

Actual observation:

Document the relevant headers visible in my screenshot.

# WAF Detection
Command
wafw00f networkwalks.com
Purpose

wafw00f was used to determine whether a Web Application Firewall could be detected.

Evidence

📸 Screenshot:
evidence/PM1-WAFW00F.png

Observation

The tool provided a WAF detection result based on the target's response behavior.

Actual result:

Document the result shown in my evidence.

# DNSRecon
Command
dnsrecon -d networkwalks.com
Purpose

DNSRecon was used to gather DNS-related information associated with the domain.

Evidence

📸 Screenshot:
evidence/PM1-DNSRecon.png

Observation

The tool returned DNS-related records and information.

Actual observation:

Document the relevant records from my own output.

# W2-PM2 — Google Hacking Database
Overview

This module introduced search-engine-based reconnaissance and the Google Hacking Database (GHDB).

The activity demonstrates how search engines can index information that organizations unintentionally expose publicly.

Objectives
Understand search-engine reconnaissance.
Learn how search operators can narrow search results.
Identify publicly indexed information.
Understand the security implications of information exposure.
Activities
Search Operators

Examples of reconnaissance operators studied include:

site:
intitle:
inurl:
filetype:
Evidence

📸 Screenshots:

evidence/PM2-GHDB-01.png
evidence/PM2-GHDB-02.png
Findings

Actual finding:

Document only the information observed during the completed laboratory exercise.

Security Relevance

Search-engine reconnaissance demonstrates that attackers may obtain useful information without directly interacting with internal systems.

This highlights the importance of:

Proper information exposure management
Secure website configuration
Removal of unnecessary public files
Monitoring publicly indexed information

# W2-PM4 — Footprinting with theHarvester
Overview

theHarvester is an OSINT tool used to gather publicly available information from supported sources.

Objectives
Perform open-source information gathering.
Identify publicly available information related to the authorized target.
Understand how different sources contribute to reconnaissance.
Document the results obtained during the exercise.
Activity

The assigned theHarvester reconnaissance workflow was performed against the authorized target.

Evidence

📸 Screenshots:

evidence/PM4-theHarvester-01.png
evidence/PM4-theHarvester-02.png
Findings

Actual findings:

Add the information observed from my own theHarvester output.

Security Relevance

OSINT tools demonstrate how information from publicly available sources can be combined during reconnaissance.

Organizations should regularly review what information is publicly exposed because individually harmless information can become more useful when combined.

# W2-PM5 — Network Scanning with Zenmap
Overview

Zenmap is the graphical interface for Nmap and can be used to perform network discovery and visualize scan results.

The assigned exercise focused on identifying the local IP address and subnet, discovering live hosts, identifying IP and MAC addresses, and generating a network topology.

# Zenmap Installation

Download and install Zenmap on the authorized Windows PC.

# Network Topology

Zenmap's topology feature was used to visualize the discovered network environment.

Evidence


evidence/PM5-Network-Topology.png
Topology File
outputs/PM5-Network-Topology.pdf

# Findings & Observations
Reconnaissance Findings

The Week 2 activities demonstrated that different reconnaissance tools expose different categories of information.

Information Type	Tool
Domain registration information	WHOIS
Web technologies	WhatWeb
DNS information	NSLookup
HTTP headers	cURL
WAF detection	wafw00f
DNS records	DNSRecon
Search-engine intelligence	GHDB
Visual OSINT	Maltego
Public information gathering	theHarvester
Network Discovery Findings

The Zenmap exercise demonstrated how network discovery can reveal:

Live hosts
IP addresses
MAC addresses
Network relationships
Network topology

The actual results are documented using evidence collected from the authorized laboratory environment.

# Problems Encountered & Troubleshooting
Maltego Configuration Issue
Problem

The assigned Maltego email-related reconnaissance transform could not be completed because the required search-engine configuration was not available.

# Investigation

The transform required additional configuration before it could return the expected information.

# Action Taken

The issue was documented rather than presenting unverified results.

# Result

The activity was recorded as Partial.

# Lesson Learned

Security tools often rely on external services, configurations, APIs, or data providers. Troubleshooting these dependencies is an important cybersecurity skill.

# What I Learned

Through the Week 2 activities, I gained practical experience in:

Reconnaissance
Domain footprinting
DNS reconnaissance
Web reconnaissance
Technology fingerprinting
HTTP header analysis
WAF detection
OSINT
Search-engine reconnaissance
Public information gathering
Relationship-based information analysis
Understanding information exposure
Network Security
Network discovery
Host identification
IP address identification
MAC address identification
Network topology visualization
Technical Skills
Kali Linux command-line usage
Nmap / Zenmap
Linux security tools
Windows networking commands
Evidence collection
Technical documentation
Professional Skills
Troubleshooting
Structured reporting
Evidence-based documentation
Security awareness
Ethical cybersecurity practice

# Security & Ethical Considerations

All activities documented in this repository are intended for authorized educational and professional cybersecurity purposes.

Reconnaissance and network scanning techniques should only be performed against systems and networks where explicit authorization has been provided.

This project does NOT include:
Passwords
API keys
Authentication tokens
Private credentials
Unauthorized access
Destructive testing

Sensitive information should be removed or redacted before publicly sharing screenshots or other evidence.

# Evidence Documentation

Evidence collected during the laboratory activities is organized by module.

# Skills Demonstrated
<p align="center">

Kali Linux
Reconnaissance
Footprinting
OSINT
DNS Enumeration
Web Reconnaissance
Network Scanning
Nmap / Zenmap
Technical Documentation
Cybersecurity Troubleshooting

</p>

# Key Commands Practiced
# WHOIS
whois networkwalks.com

# Web technology fingerprinting
whatweb networkwalks.com

# DNS lookup
nslookup networkwalks.com

# HTTP header inspection
curl -I https://networkwalks.com

# WAF detection
wafw00f networkwalks.com

# DNS enumeration
dnsrecon -d networkwalks.com

# Professional Takeaway

The Week 2 exercises demonstrated an important principle in cybersecurity:

Effective security assessment begins with understanding what information and systems are visible before attempting deeper testing.

Reconnaissance provides the foundation for later security assessment activities by helping identify the technologies, infrastructure, services, and hosts that may require further security review.

# 👤 Author
Jerose N. Aban

Cybersecurity Professional B083F — Networkwalks

# Project Status

Week 2 — Reconnaissance, Footprinting & Network Discovery

# Completed Areas

| Area | Status |
|---|---|
| Kali Linux reconnaissance | ✅ Completed |
| Domain footprinting | ✅ Completed |
| DNS reconnaissance | ✅ Completed |
| Web technology identification | ✅ Completed |
| HTTP header analysis | ✅ Completed |
| WAF detection | ✅ Completed |
| DNS enumeration | ✅ Completed |
| GHDB reconnaissance | ✅ Completed |
| theHarvester | ✅ Completed |
| Zenmap network discovery | ✅ Completed |
| Network topology documentation | ✅ Completed |
