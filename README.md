🔐 Cybersecurity Internship – Footprinting & Network Scanning

This repository documents my Week 2 Cybersecurity Internship practical work, focused on reconnaissance, footprinting, Google Dorking, and network discovery.

The activities were completed as part of an authorized cybersecurity training exercise. Testing was performed only against the assigned target and my own local network.

📌 Project Overview

Objectives

Perform passive reconnaissance and footprinting of the assigned domain.

Identify publicly available domain and web-technology information.

Inspect HTTP response headers.

Identify the presence of a Web Application Firewall (WAF).

Enumerate DNS records.

Perform Google Dorking for publicly indexed information.

Use TheHarvester for passive information gathering.

Discover live hosts on my own local network using Zenmap/Nmap.

Document observations and security considerations.

🎯 Authorized Scope

Target: networkwalks.com

Local Network: My own LAN

The activities were performed as part of an internship/training assignment with authorization. No exploitation, brute-force attacks, denial-of-service activity, or unauthorized access was performed.

Ethical & Legal Notice:
This repository is for educational and defensive-security learning purposes. Do not use these techniques against systems without explicit authorization.

🛠️ Tools Used

Tool

Purpose

WHOIS

Domain registration and name-server information

WhatWeb

Web technology and CMS fingerprinting

Nslookup

DNS resolution and IP lookup

cURL

HTTP response/header inspection

Wafw00f

WAF detection and fingerprinting

DNSRecon

DNS record enumeration

TheHarvester

Passive OSINT for emails, hosts and sub-domains

Google Dorking

Searching publicly indexed information using advanced operators

Zenmap / Nmap

Local network discovery and live-host scanning

Windows CMD

Local IP and network information

Kali Linux

Reconnaissance and security-testing environment

Windows

Google Dorking and Zenmap activities

🔎 Reconnaissance Workflow

The practical workflow followed this general sequence:

Target Identification
        ↓
WHOIS
        ↓
WhatWeb
        ↓
Nslookup
        ↓
cURL
        ↓
Wafw00f
        ↓
DNSRecon
        ↓
Google Dorking
        ↓
TheHarvester
        ↓
Zenmap / Nmap
        ↓
Documentation & Risk Analysis

💻 Commands Practiced

WHOIS

whois networkwalks.com

Used to collect publicly available domain registration and name-server information.

WhatWeb

whatweb networkwalks.com

Used to identify publicly exposed web technologies and CMS-related information.

Nslookup

nslookup networkwalks.com

Used to resolve the domain and inspect DNS resolution information.

cURL

curl -I https://networkwalks.com

Used to inspect HTTP response headers and other server-response information.

Wafw00f

wafw00f networkwalks.com

Used to identify whether a Web Application Firewall was detected.

DNSRecon

dnsrecon -d networkwalks.com

Used to enumerate DNS-related records such as NS, MX, TXT and SRV information.

TheHarvester

Example:

theHarvester -d <authorized-domain> -l 50 -b all

Used for passive information gathering from supported public sources.

Zenmap / Nmap

For my own local network:

nmap -sn <your-local-subnet>

The same activity was performed through the Zenmap GUI using a Ping Scan.

Google Dorking

Example operators practiced during the training:

site:example.com
filetype:pdf
intitle:
inurl:

Google Dorking was used only for finding publicly indexed information within the assigned educational scope.

📊 Key Learning Outcomes

Footprinting

I learned how different reconnaissance tools provide different types of information:

WHOIS → domain registration information

WhatWeb → web-technology fingerprinting

Nslookup → DNS resolution

cURL → HTTP headers and response information

Wafw00f → WAF fingerprinting

DNSRecon → DNS infrastructure information

TheHarvester → passive OSINT collection

Network Discovery

Using Zenmap/Nmap, I practiced:

Identifying my local IP and subnet

Discovering live hosts

Observing IP and MAC address information

Visualizing the local network using Zenmap topology

Security Awareness

The exercise demonstrated that publicly available information can help build an understanding of an environment before any exploitation is attempted.

These observations should not automatically be treated as confirmed vulnerabilities. Further authorized validation would be required before classifying an issue as a vulnerability.

📁 Repository Structure

This repository contains 8 screenshots and 4 supporting documents from the internship practical work.

cybersecurity-week2-footprinting/
│
├── README.md
│
├── screenshots/
│   ├── screenshot-01.png
│   ├── screenshot-02.png
│   ├── screenshot-03.png
│   ├── screenshot-04.png
│   ├── screenshot-05.png
│   ├── screenshot-06.png
│   ├── screenshot-07.png
│   └── screenshot-08.png
│
└── documents/
    ├── document-01.pdf
    ├── document-02.pdf
    ├── document-03.pdf
    └── document-04.pdf

Replace the placeholder filenames above with your actual filenames before publishing.

📸 Screenshots

The repository includes 8 screenshots showing practical evidence from the exercises.

#

Evidence

01

WHOIS / domain reconnaissance

02

WhatWeb web-technology fingerprinting

03

Nslookup DNS resolution

04

cURL HTTP-header inspection

05

Wafw00f WAF detection

06

DNSRecon DNS enumeration

07

TheHarvester / passive OSINT

08

Zenmap / Nmap local-network discovery

These screenshots are intended to document the practical work. Review each image before publishing and remove or redact any sensitive information such as credentials, cookies, tokens, private IP information, or personal data.

📄 Supporting Documents

The repository also contains 4 documents related to the internship/project.

documents/
├── document-01.pdf
├── document-02.pdf
├── document-03.pdf
└── document-04.pdf

Use descriptive filenames when uploading them, for example:

documents/
├── authorization-letter.pdf
├── week2-project-module-report.pdf
├── final-report.pdf
└── internship-task-document.pdf

Only use the names that match your actual files.

🔗 Evidence & Documentation

The screenshots and documents are included so that the repository shows both:

Practical execution evidence — screenshots of the tools and commands used.

Written documentation — project instructions, reports, authorization material, and other internship documents.

The repository is intended to demonstrate the learning process rather than publish sensitive target information.

⚠️ Responsible Disclosure & Safety

All reconnaissance and scanning activities should be performed only where authorization exists.

This project does not include:

Exploitation

Credential attacks

Brute force

Denial of service

Privilege escalation

Unauthorized access

Data modification or deletion

🎓 Internship Information

Program: Cybersecurity Internship – Networkwalks
Week: 02
Focus: Footprinting, Reconnaissance, Google Dorking & Network Scanning

Author: Shahabas Usman Ak
Role: Cybersecurity Professional / Intern

LinkedIn:
https://www.linkedin.com/in/shahabas-ak/

📚 What I Learned

This project helped me understand the importance of reconnaissance in cybersecurity and how information from different sources can be combined to build an initial picture of an environment.

I also learned the importance of:

Staying within an authorized scope

Recording evidence clearly

Separating observations from confirmed vulnerabilities

Writing security findings in a professional format

Protecting sensitive information when publishing technical work

⭐ Future Improvements

Future versions of this project can include:

More structured reconnaissance notes

Automated evidence collection

Improved reporting templates

Additional defensive analysis

Lab-based vulnerability validation on intentionally vulnerable systems

🔐 Disclaimer

This repository is intended for educational cybersecurity practice and authorized security testing only.

Use these techniques only on systems you own or have explicit permission to test.
