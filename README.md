# Network Reconnaissance & VAPT Assessment

This repository documents a reconnaissance and enumeration exercise performed against an authorized public test target, scanme.org. The project follows the information-gathering phase of a typical VAPT engagement and includes passive OSINT, subdomain discovery, service enumeration, web directory enumeration, and a written assessment report.

## Project Overview

This mini-project demonstrates a structured reconnaissance workflow using both passive and active techniques. It focuses on identifying publicly exposed assets, mapping the external attack surface, and documenting the findings in a professional report.

## Objective

To simulate the first phase of a real-world penetration test by collecting publicly available information about a target, enumerating exposed services and subdomains, and reporting the results with recommendations.

## Scope

The assessment was limited to non-invasive reconnaissance and enumeration only:

- No exploitation was performed
- No denial-of-service actions were carried out
- No unauthorized access attempts were made

## Target

- Target: scanme.org
- Authorization: Public test target maintained by the Nmap Security Scanner Project
- Assessment date: 7 July 2026

## Methodology

1. Passive reconnaissance using WHOIS, Netcraft, and Shodan
2. Subdomain enumeration using Subfinder
3. Port and service identification using Nmap
4. Web directory enumeration using Gobuster
5. Documentation of findings and risk assessment in the report

## Tools Used

- WHOIS
- Netcraft
- Shodan
- Subfinder
- Nmap
- Gobuster

## Key Findings

- 17 subdomains discovered
- 2 open ports identified by Nmap (SSH on port 22 and HTTP on port 80)
- Shodan also showed additional exposed services such as port 123/UDP and port 31337/TCP
- Gobuster found publicly accessible administrative-style endpoints such as /admin and /login
- Overall exposure was assessed as Medium due to the expanded subdomain footprint and exposed endpoints

## Repository Contents

- report/: contains the project report PDF
- outputs/: contains collected output artifacts from the assessment
- screenshots/: contains screenshots captured during the workflow

## Report

The full assessment report is available here:

- [report/MINI PROJECT 1 .pdf](report/MINI%20PROJECT%201%20.pdf)

## Screenshots

Screenshots captured during the project are stored in the [screenshots](screenshots) folder.

## Disclaimer

This assessment was performed only against explicitly authorized targets and is intended for educational and academic purposes.

