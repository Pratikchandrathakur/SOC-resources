# SOC Tools and Their Features
A SOC relies on a supporting infrastructure of tools and systems that provide the following services:
- Network mapping
- Network monitoring
- Vulnerability detection
- Penetration testing
- Data collection
- Threat and anomaly detection 
- Data aggregation and correlation
### One tool that is used by analysts in a SOC is Security Onion.

<b>Security Onion</b> is intended to support SOC analysts with a suite of tools for network security monitoring, including intrusion detection, network security monitoring, and log management. The Security Onion distribution is based on the Ubuntu Linux operating system and contains several useful security tools that are designed to provide four core network security-monitoring functions as follows:

1. Full packet capture
2. Network-based and host-based intrusion detection sensors
3. Security analysis tools
4. Log management

## The Enterprise Log Search and Archive (ELSA) version of Security Onion is composed of the following tools: 

- ELSA: ELSA is a centralized syslog framework that is built on Syslog-NG, MySQL, and Sphinx full-text search. It provides a fully asynchronous web-based query interface that normalizes logs and makes searching billions of them for arbitrary strings as easy as searching the web. It also includes tools for assigning permissions for viewing the logs, email-based alerts, scheduled queries, and graphing.

- Snort: An open source, rules-driven network intrusion detection system (NIDS) and network intrusion prevention system (NIPS) developed by Cisco (Sourcefire). It performs real-time threat detection and generates alerts when threats are detected. The NIPS inline mode is not supported within Security Onion.

- Suricata: A script-driven NIDS and NIPS threat detection engine for analyzing traffic and generating alerts. NIPS inline mode is not supported within Security Onion.

- Zeek (Bro): A packet recorder and protocol parsing engine that is commonly used to analyze network traffic to detect behavioral anomalies.

- Traffic logging: Traffic captured by means of SPAN, a TAP port, or a packet broker. Traffic logging generates comprehensive, protocol-specific traffic logs for more than 35 network protocols and application layer analyzers, including HTTP, DNS FTP, and SMTP.

- Automated analysis: Traffic analysis that uses Bro scripts.

- File extraction: Extracts and reassembles various file types directly off the wire.

- Wazuh (OSSEC): Host-based intrusion detection system (HIDS) that replaced OSSEC and is used to monitor and defend Security Onion. Wazuh offers a lightweight monitoring agent that can be installed on network host devices and is supported on Windows, Linux, Mac OS X, HP-UX, AIX, and Solaris platforms.

- Netsniff-ng: Captures network traffic via SPAN, a TAP port, or packet broker in the form of PCAP files.

- Sysmon: Windows system service to monitor event log and system activity.

- Syslog-ng: An enhanced BSD log daemon that can receive logs and collect inputs from a wide range of sources.

- Network analyst tools: Provide packet capture and network traffic IP flow analytics capabilities that can be used to find anomalous network activity. The following popular network analyst tools are included within Security Onion:

- Wireshark: Network protocol analyzer

- Sguil: Sguil (pronounced "sgweel") is built by network security analysts for network security analysts. Sguil's main component is an intuitive GUI that provides access to real-time events, session data, and raw packet captures. Sguil facilitates the practice of Network Security Monitoring and event driven analysis.

- Squert: Squert is a web application that is used to query and view event data that is stored in a Sguil database (typically IDS alert data). Squert is a visual tool that attempts to provide additional context to events by using metadata, time series representations and weighted and logically grouped result sets.

- NetworkMiner: Performs network traffic analysis for parsing PCAP files and extracting artifacts

- CyberChef: Web-based application for data manipulation

- CapME: Helps with analyzing PCAP transcripts and downloading captured PCAP files

<b>The preceding tools are included in Security Onion to aid the SOC analyst in viewing network telemetry data and analyzing that data to determine if a network intrusion has occurred. For example, IDS alerts are generated from Snort or Suricata. A SOC analyst could use ELSA to query log data from other sources to validate alert messages that are from Snort. Sguil is a real-time event- and session-monitoring tool that displays data for a SOC analyst to interpret. These types of tools are used by security analysts to perform their jobs.</b>

## A newer release of Security Onion is called the Elastic Stack (ELK) version. It includes the following tools:

- Elasticsearch: Ingest and index logs, large scalable search engine based on Apache Lucene

- Logstash: Data ingestion engine, parsing, and format logs

- Kibana: Web dashboard that offers visualizations of ingested log data and data exploration. (Kibana and Squert can pivot to CapMe to retrieve full packet captures.)

- TheHIVE: Security incident response platform and case management system integrated with Malware Information Sharing Platform (MISP)

- Elastic Beats: Lightweight data shipper server agent that sends specific types of operational data to Logstash and Elasticsearch

- Curator: Manage indices through scheduled maintenance

- ElastAlert: Query Elasticsearch and alert on user-defined anomalous behavior or other interesting bits of information

- FreqServer: Detect DGAs and find random filenames, script names, process names, service names, workstation names, TLS certificate and issuer subjects, and so on.

- DomainStats: Conducts whois lookups and provides info about a domain by providing additional context, such as creation time, age, reputation.

## The following figure shows the relationship between the Security Onion 2 Elastic Stack components.



