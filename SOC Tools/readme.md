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

This suite of tools enables SOC analysts to collect, analyze, and visualize network data to detect and respond to intrusions effectively.  
