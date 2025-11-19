📡 IP Threat Investigation & OSINT Analysis

A hands-on threat investigation project analyzing suspicious IP addresses using OSINT tools, DNS lookups, malware feeds, and threat-intel enrichment.
This lab simulates real SOC workflows: pivoting on an IP, validating reputation, extracting metadata, and correlating findings across multiple sources.
🔍 What This Investigation Covers
1. DNS & Network Enumeration

nslookup, dig, host

A/AAAA records

Mail, TXT, and NS records

DNS path tracking

2. Threat Intelligence Lookups

Correlated IP reputation using:

VirusTotal

Cisco Talos Intelligence

AbuseIPDB

AlienVault OTX

IP geolocation APIs

IP2Location

ipregistry.co

3. API-Based Data Collection

Queried threat intel sources using curl:

curl -s "https://ipinfo.io/<IP>?token=<TOKEN>"


Extracted:

ASN

Organization

Country

Hosting provider

Known malware associations

Sandbox detections

4. Geolocation & Network Attribution

Validated IP origin using:

IP2Location

ipinfo

ipregistry

MaxMind-style lookups

Mapped:

Lat/Long

ISP

Region

Hosting type (proxy, VPN, data center)

🧠 Methodology Summary

Selected suspicious IPs from threat feeds (OTX, Talos, etc.)

Ran DNS enumeration (dig, nslookup, host)

Queried IP reputation via API and browser tools

Extracted ASN + org metadata

Cross-check geolocation sources

Correlated any malware signatures

Documented indicators in /findings

📁 Repository Structure
/screenshots   → all investigation terminal/web screenshots
/findings      → summarized notes, indicators, JSON samples
README.md      → project explanation & methodology
queries.txt    → all commands used in the investigation

🚀 How to Use This Repo

Clone it:

git clone https://github.com/Niknaz-65/<REPO-NAME>.git


Review:

/screenshots → all OSINT evidence

/findings → conclusions and indicator summaries

👩‍💻 Author

Niknaz Sadehvandi
Cybersecurity Student | SOC Analyst Learner | Threat Intelligence & OSINT Enthusiast
🔗 LinkedIn: https://www.linkedin.com/in/niknaz-sadehvandi-a34179325/
