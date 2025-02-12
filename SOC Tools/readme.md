# **🔒 SOC Tools and Their Features**  
A Security Operations Center (SOC) relies on a range of tools and systems to support its functions. These tools provide the following core services:

- 🌐 **Network mapping**  
- 📡 **Network monitoring**  
- 🔍 **Vulnerability detection**  
- 🛡️ **Penetration testing**  
- 📊 **Data collection**  
- 🚨 **Threat and anomaly detection**  
- 📑 **Data aggregation and correlation**  

---

### **🛠️ Security Onion**  
Security Onion is a comprehensive suite of tools designed to assist SOC analysts with network security monitoring, intrusion detection, and log management. Built on Ubuntu Linux, Security Onion offers four core network security-monitoring functions:  

1. 📁 **Full packet capture**  
2. 🖥️ **Network-based and host-based intrusion detection sensors**  
3. 🔎 **Security analysis tools**  
4. 🗃️ **Log management**  

---

## **📦 Security Onion (ELSA Version)**  
The Enterprise Log Search and Archive (ELSA) version of Security Onion includes the following tools:  

- 📋 **ELSA:** Centralized syslog framework with web-based query interfaces for log normalization and searches. Features include log permissions, email alerts, scheduled queries, and graphing.  
- 🛡️ **Snort:** Open-source NIDS/NIPS for real-time threat detection and alerting (NIPS mode not supported in Security Onion).
 <img align=left src="https://github.com/user-attachments/assets/8c962191-3f55-47fc-817d-a3b8211cbf74">
 
- 📜 **Suricata:** Script-driven NIDS/NIPS for traffic analysis and alert generation (NIPS mode not supported).  
- 🔍 **Zeek (Bro):** Packet recorder and protocol analyzer to detect behavioral anomalies.  
   - 🌐 **Traffic Logging:** Captures comprehensive traffic logs for over 35 protocols (e.g., HTTP, DNS, SMTP).  
   - ⚙️ **Automated Analysis:** Uses Bro scripts for traffic analysis.  
   - 📂 **File Extraction:** Reassembles files directly from network traffic.  
- 🛡️ **Wazuh (OSSEC):** Host-based intrusion detection system for lightweight host monitoring on multiple OS platforms.  
- 📦 **Netsniff-ng:** Captures network traffic in PCAP format.  
- 🖥️ **Sysmon:** Monitors Windows event logs and system activity.  
- 📤 **Syslog-ng:** Enhanced BSD log daemon for log collection from diverse sources.  

### **🧰 Network Analyst Tools**  
Security Onion includes powerful network analyst tools for packet capture and anomaly detection:

- 📡 **Wireshark:** Network protocol analyzer.  
- 📊 **Sguil:** Real-time event and session monitoring GUI for SOC analysts.  
- 📈 **Squert:** Web application for querying event data with metadata and time series visualizations.  
- 🗂️ **NetworkMiner:** PCAP file parser and artifact extractor.  
- 🧪 **CyberChef:** Web-based data manipulation tool.  
- 📁 **CapME:** Tool for analyzing PCAP transcripts and downloading captured PCAP files.  

These tools help SOC analysts visualize network data and detect intrusions. For instance, Snort alerts can be validated using ELSA, and Sguil provides real-time event data for deeper analysis.

---

## **📦 Security Onion (Elastic Stack Version)**  
A newer release of Security Onion includes the Elastic Stack (ELK) version, which features:  

- 📦 **Elasticsearch:** Scalable log indexing and search engine.  
- 🛠️ **Logstash:** Data ingestion engine for log parsing and formatting.  
- 📊 **Kibana:** Web dashboard for log visualization and data exploration (can pivot to CapME for packet capture retrieval).  
- 📂 **TheHIVE:** Incident response and case management platform integrated with MISP.  
- 📤 **Elastic Beats:** Lightweight data shippers for sending operational data to Logstash and Elasticsearch.  
- 🗄️ **Curator:** Manages indices with scheduled maintenance tasks.  
- 🚨 **ElastAlert:** Queries Elasticsearch for anomalies and triggers alerts.  
- 🔍 **FreqServer:** Detects DGAs and identifies random file, process, service, and domain names.  
- 🌐 **DomainStats:** Conducts Whois lookups and provides domain context (e.g., age, reputation).  

---
 <img align=left src="https://github.com/user-attachments/assets/c2e45d7a-0181-4243-a672-993bdea1972a">
 
---

This suite of tools enables SOC analysts to collect, analyze, and visualize network data to detect and respond to intrusions effectively.  
# **🔒 SOC Tools and Their Features (Cont.)**  

You might use other tools, besides Security Onion, such as the following:

---

### **🔍 Cisco Secure Network Analytics (formerly Stealthwatch)**  
Displays distinct views of the IP flows traversing network devices that are configured to send NetFlow data to Cisco Secure Network Analytics. It uses NetFlow, IPFIX, and other types of network telemetry data to detect a wide range of threats such as:

 <img align=left src="https://github.com/user-attachments/assets/f07f4d1f-f4ab-4a51-830a-14aade2028e8">

- 🛡️ Advanced persistent threats (APT)  
- 📶 Distributed denial of service (DDoS) attacks  
- 🐛 Zero-day malware  
- 👤 Insider threats  

Cisco Secure Network Analytics applies various behavior and policy-based algorithms to alarm SOC analysts about suspicious behavior on the network.  

---

### **🔬 Cisco Secure Malware Analytics (formerly Threat Grid)**  
A cloud-based malware analysis and threat intelligence sandbox solution. A SOC analyst can submit malware samples for analysis during an investigation.  

 <img align=left src="https://github.com/user-attachments/assets/e2337f7c-8846-4628-a595-db29975e9af5">

- 🔍 Uses various static and dynamic analysis engines to dissect file behaviors to determine whether a file might be malicious.  
- 🌍 Correlates data elements of a single malware sample against millions of samples collected worldwide.  
- 🔗 Provides a global view of malware attacks and their associations.  

Cisco Secure Malware Analytics is included as an integrated component of many Cisco Secure products.  

---

### **🔗 Cisco SecureX Platform**  
Connects the Cisco integrated security portfolio with the organization's entire security infrastructure. 

<img src="https://github.com/user-attachments/assets/213b447f-15dc-4bca-995c-e50e17368510" width=1000px>

- 📊 Provides a consistent experience that unifies visibility and identifies unknown threats.  
- ⚙️ Enables automated workflows to strengthen security across the network, endpoint, cloud, and applications.  
- 🌐 An open, cloud-native platform included with many Cisco Secure products.  
- 🤝 Aligns with products from more than 175 security technology providers and offers more than 300 product-to-product integrations.  

---

### **🛡️ Penetration Testing Tools**  
Penetration testing simulates the actions of an attacker aiming to breach an organization’s information security.  

- 🎯 The penetration tester (ethical hacker) uses various tools and techniques to exploit critical systems and gain access to sensitive data.  
- 🧪 A vulnerability assessment identifies known vulnerabilities in information systems and reports potential exposures.  
- 🔄 Organizations typically start with vulnerability assessments and act on the results to reduce risks before conducting penetration tests.  

**🔧 Common Penetration Testing Tools:**  
- **Metasploit Framework**  
- **Armitage**  
- **Social Engineer Toolkit (SET)**  
 <img align=left src="https://github.com/user-attachments/assets/a6a57fa5-b9b3-4fcb-bf7e-721bf81fffc8">

Kali Linux contains many penetration testing tools for security and forensics fields. For example, using Armitage to exploit the Apache Struts vulnerability can open a reverse connection to a vulnerable Apache server (192.168.1.107).  

---

In the following figure, the `whoami` command is issued after the reverse connection is established. 

 <img align=left src="https://github.com/user-attachments/assets/427852f8-fb00-4cd8-82d6-d258773f935b">
