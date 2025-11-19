# 🌐 IP Threat Investigation & OSINT Analysis

A hands-on threat investigation project analyzing suspicious IP addresses using OSINT tools, DNS lookups, API enrichment, and threat-intel feeds.  
This project simulates real SOC and CTI workflows by pivoting on an IP, verifying reputation, extracting metadata, and correlating evidence across multiple sources.

---

## 🔍 Investigation Techniques

### **1. Network & DNS Enumeration**
Used the following tools to extract DNS and network metadata:
- `whois`
- `nslookup`
- `dig`
- `host`

Collected:
- A/AAAA records  
- TXT / MX / NS records  
- Reverse DNS  
- Registrar & ASN details  

---

### **2. Threat Intelligence Lookups**
IP reputation checked using:
- VirusTotal  
- Cisco Talos  
- AbuseIPDB  
- OTX lookups  
- Passive DNS  
- Threat feed metadata  

---

### **3. API-Based Enrichment**
Queried IP intelligence APIs using `curl`:

```bash
curl -s "https://ipinfo.io/<IP>?token=<TOKEN>"
```

Extracted:
- ASN  
- Organization  
- Country  
- Region  
- Hosting type (VPN, proxy, datacenter)  
- Known malware associations  

---

## 🧠 Methodology Summary

1. Selected suspicious IP from threat feeds  
2. Ran whois & DNS enumeration  
3. Queried reputation from multiple OSINT sources  
4. Pulled metadata via API  
5. Mapped IP geolocation details  
6. Correlated ASN + hosting provider + malware flags  
7. Compiled evidence in screenshots & findings  

---

## 🖼️ Screenshots (Evidence)

All screenshots stored in `/screenshots/`.

### **1. Whois lookup**
![Whois Result](screenshots/Screenshot%202025-04-27%20113820.png)

### **2. Reverse DNS**
![Reverse DNS](screenshots/Screenshot%202025-04-27%20113935.png)

### **3. Geolocation Information**
![Geo IP](screenshots/Screenshot%202025-04-27%20114100.png)

### **5. Additional IP Intel Panel**
![IP Panel](screenshots/Screenshot%202025-05-01%20092404.png)

### **6. Terminal whois output**
![Whois Terminal](screenshots/Screenshot%202025-05-05%20100544.png)

### **7. DNS Records**
![DNS Lookup](screenshots/Screenshot%202025-05-05%20100813.png)

### **8. ASN + Organization**
![ASN Lookup](screenshots/Screenshot%202025-05-06%20134340.png)

### **9. API Response JSON**
![API JSON](screenshots/Screenshot%202025-05-06%20134433.png)

### **10. Additional DNS Metadata**
![DNS Metadata](screenshots/Screenshot%202025-05-06%20152708.png)

---

## 📁 Repository Structure

```
/screenshots     → all investigation evidence  
/findings        → JSON metadata, notes, report  
queries.txt      → all commands used  
README.md        → project documentation
```

---

## 🚀 Clone This Project

```bash
git clone https://github.com/Niknaz-65/ip-threat-investigation.git
```

---

## 👩‍💻 Author

**Niknaz Sadehvandi**  
Cybersecurity Student | SOC Analyst Learner | OSINT & Threat Intelligence Enthusiast  
🔗 LinkedIn: https://www.linkedin.com/in/niknaz-sadehvandi-a34179325/
