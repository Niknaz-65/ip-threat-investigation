# IP Threat Investigation & OSINT Analysis

## Overview
Threat intelligence investigation focused on analyzing a suspicious IP address using OSINT techniques, DNS enumeration, API-based enrichment, and threat-intel correlation to support SOC and CTI workflows.

## Why This Project Matters to SOC Teams
- Enables rapid assessment of suspicious IPs during alerts and investigations
- Supports triage decisions by validating reputation, hosting type, and threat associations
- Produces enriched indicators suitable for blocking, monitoring, or escalation

## Environment
- OS: Linux / Windows
- Tools: whois, nslookup, dig, host, curl
- Threat Intelligence Sources: VirusTotal, Cisco Talos, AbuseIPDB, AlienVault OTX
- APIs: ipinfo.io
- Frameworks: Threat Intelligence lifecycle, SOC triage workflow

## Data Collected / Artifacts
- IP address metadata
- DNS records (A, PTR, MX, NS, TXT)
- ASN and hosting provider details
- Geolocation data
- Reputation scores and threat flags
- API JSON responses

## Analysis Steps
1. Selected a suspicious IP from threat intelligence sources
2. Performed whois and DNS enumeration
3. Queried multiple reputation and threat-intel platforms
4. Enriched IP metadata using REST APIs
5. Correlated ASN, hosting provider, and abuse indicators
6. Documented findings with screenshots and structured notes

## Findings
- IP associated with hosting infrastructure commonly used for malicious activity
- Reputation data indicated elevated abuse reports
- ASN and provider analysis supported non-residential usage
- DNS and reverse-lookup behavior consistent with suspicious infrastructure

## Outcome
- IP classified as high-risk
- Indicator suitable for blocking or heightened monitoring
- Recommended correlation with firewall, proxy, and SIEM logs

## Screenshots / Evidence

All evidence stored in `/screenshots/`.

### Whois Lookup
![Whois Result](screenshots/Screenshot%202025-04-27%20113820.png)

### Reverse DNS
![Reverse DNS](screenshots/Screenshot%202025-04-27%20113935.png)

### Geolocation Information
![Geo IP](screenshots/Screenshot%202025-04-27%20114100.png)

### Threat Intelligence Panels
![IP Intel](screenshots/Screenshot%202025-05-01%20092404.png)

### API Response (JSON)
![API JSON](screenshots/Screenshot%202025-05-06%20134433.png)

## Repository Structure
```text
/screenshots   → investigation evidence  
/findings      → metadata, notes, reports  
queries.txt    → executed commands  
README.md      → project documentation
```
## Author
**Niknaz Sadehvandi**  
**Cybersecurity Analyst**  
LinkedIn: https://www.linkedin.com/in/niknaz-sadehvandi-a34179325/

