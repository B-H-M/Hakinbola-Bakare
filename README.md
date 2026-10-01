# 🛡️ Cybersecurity Learning Journey

## Overview

This repository documents my ongoing hands-on cybersecurity learning and development through the **LetsDefend Blue Team training environment**.

My current focus is developing the technical foundation required for **Security Operations Center (SOC), Security Analyst, and Incident Response roles**.

Rather than simply completing courses, my objective is to understand how networks, operating systems, security technologies, malware, logs, and alerts interact during real security investigations.

---

## 📑 Table of Contents

- [🌐 1. Network Fundamentals](#-1-network-fundamentals)
- [🔗 2. Network Fundamentals II](#-2-network-fundamentals-ii)
- [🪟 3. Windows Fundamentals](#-3-windows-fundamentals)
- [🐧 4. Linux for Blue Team](#-4-linux-for-blue-team)
- [📡 5. Network Protocols](#-5-network-protocols)
- [🌍 6. Network Protocols II](#-6-network-protocols-ii)
- [🔐 7. Introduction to Cryptology](#-7-introduction-to-cryptology)
- [🦠 8. Malware Analysis Fundamentals](#-8-malware-analysis-fundamentals)
- [🦠 9. Malware Traffic Analysis with Wireshark](#-9-malware-traffic-analysis-with-wireshark)
- [🔬 10. Dynamic Malware Analysis](#-10-dynamic-malware-analysis)
- [🚨 11. How to Investigate a SIEM Alert](#-11-how-to-investigate-a-siem-alert)
- [🧰 Tools & Technologies Encountered](#-tools--technologies-encountered)
- [🧠 How My Skills Connect](#-how-my-skills-connect)
- [🎯 Skills I Am Developing](#-skills-i-am-developing)
- [🚀 Current Objective](#-current-objective)
- [📚 Training Platform](#-training-platform)

---

# 🌐 1. Network Fundamentals

**Training:** LetsDefend – Network Fundamentals  
**Completed Content:** 9 lessons | 16 questions | 1 quiz

This module strengthened my understanding of how computer networks operate and why networking knowledge is essential when investigating cybersecurity incidents.

### Key Concepts Studied

#### Network Types

I developed an understanding of common network types and how systems communicate across different environments.

This includes concepts surrounding:

- LAN
- WAN
- PAN
- MAN
- Internet-based networks

Understanding network scope is important when determining where communication originates and where security controls should be positioned.

#### Network Topologies

I studied how network devices can be physically or logically arranged.

Examples include:

- Star topology
- Bus topology
- Ring topology
- Mesh topology

From a security perspective, network topology helps an analyst understand traffic paths and identify where monitoring or security devices may exist.

#### OSI Model

I developed a working understanding of the seven layers of the OSI model:

1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application

I learned to associate networking technologies and protocols with their respective layers.

For example:

- Ethernet → Data Link
- IP → Network
- TCP/UDP → Transport
- HTTP/DNS → Application

The OSI model provides a useful troubleshooting framework because network problems and security events can be analyzed according to the layer where they occur.

#### Network Devices

I studied the roles of devices such as:

- Switches
- Routers
- Firewalls
- Access points
- Hubs
- Gateways

I learned that switches primarily move traffic within networks using MAC addresses, while routers move traffic between networks using IP addressing and routing information.

#### TCP/IP Model

I also studied the TCP/IP model and how it relates to practical Internet communications.

The model helped me understand how application data is encapsulated, transmitted across networks and eventually delivered to the correct application on the destination system.

#### IP Addressing

I developed an understanding of:

- IPv4 addresses
- Network and host portions
- Public vs private IP addresses
- Subnet concepts
- Default gateways

This knowledge is directly relevant to SOC investigations because IP addresses frequently appear in firewall logs, authentication logs, SIEM alerts, packet captures and threat intelligence reports.

#### Network Address Translation — NAT

I learned how NAT allows private internal addresses to communicate with external networks through translated public addresses.

From a security perspective, I now understand why analysts sometimes need NAT or firewall logs to identify the actual internal device responsible for particular network activity.

---

# 🔗 2. Network Fundamentals II

**Training:** LetsDefend – Network Fundamentals II  
**Completed Content:** 11 lessons | 25 questions | 1 quiz

This module expanded my networking knowledge into concepts that are particularly important when analyzing network traffic and security events.

### Key Areas Studied

#### VLANs

I learned how **Virtual Local Area Networks (VLANs)** logically separate devices even when those devices may share the same physical switching infrastructure.

I understand that VLANs can improve:

- Network segmentation
- Traffic management
- Security boundaries

From a Blue Team perspective, segmentation can limit communication between systems and potentially reduce an attacker's ability to move laterally through an environment.

#### VPNs

I studied how Virtual Private Networks provide secure communication over untrusted networks.

VPN knowledge is particularly useful when investigating:

- Remote-user connections
- Authentication activity
- Unusual login locations
- Remote access incidents

#### MAC Addresses & ARP

I learned how MAC addresses operate at Layer 2 and how **Address Resolution Protocol (ARP)** maps IPv4 addresses to MAC addresses on local networks.

Understanding ARP also provides useful background for investigating attacks such as ARP spoofing and man-in-the-middle activity.

#### ICMP

I learned how ICMP supports network diagnostics and error reporting.

Common utilities such as `ping` and `traceroute` help identify connectivity problems and network paths.

I also understand that ICMP traffic may appear during reconnaissance and network discovery.

#### Routing

I developed a better understanding of how routers determine where packets should be forwarded when traffic must travel between networks.

---

# 🪟 3. Windows Fundamentals

**Training:** LetsDefend – Windows Fundamentals  
**Completed Content:** 14 lessons | 32 questions | 1 quiz

This module developed my understanding of Windows from a cybersecurity and Blue Team perspective.

My learning included:

- Windows operating system architecture
- Users and groups
- File systems
- Processes
- Services
- Windows administration
- Command-line utilities
- System configuration
- Windows security concepts
- Event logging

One of my key takeaways is the importance of understanding **normal system activity before attempting to identify malicious behaviour**.

This knowledge helps when examining suspicious processes, accounts, services, login activity, files, commands and system events.

---

# 🐧 4. Linux for Blue Team

**Training:** LetsDefend – Linux for Blue Team  
**Completed Content:** 13 lessons | 21 questions | 1 quiz

This module strengthened my Linux knowledge specifically from the perspective of defensive security.

I developed familiarity with:

- Linux filesystem structure
- Files and directories
- Users and groups
- Permissions
- Processes
- Services
- Networking
- Command-line navigation
- Log analysis

Useful commands encountered include:

```bash
ls
cd
pwd
cat
grep
find
ps
netstat
ss
chmod
chown
tail
head
```

These tools can help analysts locate suspicious files, inspect processes, identify network connections and examine logs.

---

# 📡 5. Network Protocols

**Training:** LetsDefend – Network Protocols  
**Completed Content:** 7 lessons | 20 questions | 1 quiz

This module helped me understand how common network protocols behave and what normal communication should look like.

Protocols studied include areas surrounding:

- HTTP/HTTPS
- DNS
- DHCP
- FTP
- SSH
- Email protocols

| Protocol | Common Port | Purpose |
|---|---:|---|
| HTTP | 80 | Web traffic |
| HTTPS | 443 | Encrypted web traffic |
| DNS | 53 | Name resolution |
| SSH | 22 | Secure remote access |
| FTP | 21 | File transfer |
| SMTP | 25 | Email transmission |

Rather than simply memorising port numbers, I am developing an understanding of how protocols behave and why unusual protocol activity can be significant during an investigation.

---

# 🌍 6. Network Protocols II

**Training:** LetsDefend – Network Protocols II  
**Completed Content:** 7 lessons | 20 questions | 1 quiz

This module expanded my understanding of network communication and how protocols can be interpreted during security investigations.

When analysing network activity, I learned to consider:

- Source IP
- Destination IP
- Source and destination ports
- Protocol
- Connection frequency
- Data transferred
- Timing
- Expected behaviour
- Threat intelligence

An important takeaway is that traffic using a legitimate protocol is **not automatically legitimate**.

---

# 🔐 7. Introduction to Cryptology

**Training:** LetsDefend – Introduction to Cryptology  
**Completed Content:** 12 lessons | 20 questions | 1 quiz

This module introduced me to the principles used to protect the confidentiality and integrity of information.

### Concepts Studied

- Encryption
- Decryption
- Plaintext
- Ciphertext
- Cryptographic keys
- Symmetric encryption
- Asymmetric encryption
- Hashing

I learned how symmetric and asymmetric encryption differ and how hashing is used for file identification, integrity verification and IOC investigation.

Common hashes encountered in cybersecurity include:

- MD5
- SHA-1
- SHA-256

---

# 🦠 8. Malware Analysis Fundamentals

**Training:** LetsDefend – Malware Analysis Fundamentals  
**Practical Content:** 7 lessons | 13 questions | 3 challenges | 1 quiz | 3 alerts

This module marked my transition from foundational cybersecurity concepts into practical security analysis.

I learned how malware analysis helps determine:

- What a suspicious file is
- What the file attempts to do
- What resources it contacts
- What system changes it makes
- Whether it represents a genuine threat
- Which Indicators of Compromise can be extracted

I studied malware categories including:

- Trojans
- Ransomware
- Worms
- Spyware
- Downloaders
- Backdoors

I also developed an understanding of **static analysis** versus **dynamic analysis**.

Potential IOCs include:

- File hashes
- IP addresses
- Domains
- URLs
- File paths
- Process activity
- Registry modifications
- Network connections

---

# 🦠 9. Malware Traffic Analysis with Wireshark

**Training:** LetsDefend – Malware Traffic Analysis with Wireshark  
**Practical Content:** 4 lessons | 5 questions | 2 challenges

This module introduced me to investigating malicious network behaviour using **Wireshark**.

I practiced analyzing:

- Source IP addresses
- Destination IP addresses
- Ports
- Protocols
- DNS requests
- HTTP communications
- TCP conversations
- Suspicious external connections

Examples of Wireshark display filters I became familiar with include:

```text
ip.addr == 192.168.1.10
dns
http
tcp
tcp.port == 443
```

The key takeaway was learning how packet captures can be used to reconstruct network activity rather than relying solely on automated alerts.

---

# 🔬 10. Dynamic Malware Analysis

**Training:** LetsDefend – Dynamic Malware Analysis  
**Practical Content:** 9 lessons | 17 questions | 2 challenges | 1 quiz | 3 alerts

Dynamic malware analysis expanded my understanding of how suspicious software can be investigated by observing its behaviour during execution.

I learned to investigate behaviour such as:

- Process creation
- Child processes
- File creation
- File modification
- Registry activity
- Network connections
- DNS requests
- External IP communication
- Persistence mechanisms

Dynamic analysis can reveal useful IOCs including:

```text
File Hash
IP Address
Domain
URL
File Path
Registry Key
Process Name
Command Line
```

I also learned the importance of conducting malware analysis within a **controlled and isolated environment**.

---

# 🚨 11. How to Investigate a SIEM Alert

**Training:** LetsDefend – How to Investigate a SIEM Alert  
**Completed Content:** 7 lessons | 20 questions

This module brought together many of the skills developed throughout my previous training.

### SIEM Investigation Workflow

```text
Alert Generated
      ↓
Review Alert Details
      ↓
Understand Detection Rule
      ↓
Identify Affected Asset/User
      ↓
Gather Relevant Evidence
      ↓
Analyze Logs / Network / Endpoint Data
      ↓
Determine True Positive or False Positive
      ↓
Assess Scope and Impact
      ↓
Document Findings
      ↓
Escalate / Contain / Close
```

### Alert Triage

When reviewing an alert, I learned to ask questions such as:

- What triggered the alert?
- Which user or endpoint is involved?
- What happened?
- When did it happen?
- What is the source?
- What is the destination?
- Is the activity expected?
- Are there related events?
- Is there evidence of malicious behaviour?

### Evidence Correlation

A key skill I am developing is correlating evidence from different security sources:

```text
SIEM Alert
     ↓
User Activity
     ↓
Endpoint Logs
     ↓
Network Logs
     ↓
IP / Domain Reputation
     ↓
Process / File Analysis
```

A single log entry may not provide enough evidence to make a decision. Correlating multiple data sources creates a clearer picture of what occurred.

### Investigation Documentation

I also learned the importance of documenting:

- Alert trigger
- Evidence reviewed
- Systems/users involved
- Indicators identified
- Analysis performed
- Investigation conclusion
- Actions taken or recommended

---

# 🧰 Tools & Technologies Encountered

| Area | Technologies / Concepts |
|---|---|
| **Networking** | TCP/IP, OSI, IPv4, MAC, ARP, ICMP, NAT, VLAN, VPN, Routing |
| **Traffic Analysis** | Wireshark, PCAP analysis, network filtering |
| **Operating Systems** | Windows, Linux |
| **Security Monitoring** | SIEM, alerts, logs, event correlation |
| **Malware Analysis** | Static analysis concepts, dynamic analysis, sandboxing |
| **Threat Investigation** | IOCs, hashes, IPs, domains, URLs |
| **Cryptography** | Encryption, hashing, symmetric/asymmetric cryptography |
| **Investigation** | Alert triage, evidence collection, validation and escalation |

---

# 🧠 How My Skills Connect

One of the biggest outcomes of this learning journey has been understanding that cybersecurity concepts do not operate independently.

```text
Networking Fundamentals
        ↓
Network Protocols
        ↓
Windows & Linux
        ↓
Logs & Network Traffic
        ↓
Security Monitoring
        ↓
SIEM Alerts
        ↓
Malware / Threat Analysis
        ↓
Incident Investigation
        ↓
Incident Response
```

For example, investigating suspicious malware communication may require me to understand:

1. The source and destination IP addresses.
2. Which protocol and ports were used.
3. DNS queries made by the endpoint.
4. Processes responsible for the connection.
5. Windows or Linux logs associated with the activity.
6. File hashes and other Indicators of Compromise.
7. Whether the behaviour matches known malicious activity.
8. Whether the SIEM alert represents a true or false positive.

This is helping me move from learning isolated cybersecurity definitions toward developing an **analyst mindset based on evidence, correlation and investigation**.

---

# 🎯 Skills I Am Developing

Through this learning path, I am actively developing skills in:

- Network traffic analysis
- TCP/IP troubleshooting
- Windows and Linux investigation
- Log analysis
- SIEM alert triage
- Security event investigation
- Malware analysis
- Dynamic malware analysis
- Wireshark packet analysis
- IOC identification
- Threat investigation
- Evidence correlation
- Incident documentation

---

# 🚀 Current Objective

My goal is to continue building practical Blue Team skills and develop the technical depth required to work effectively in roles such as:

- SOC Analyst
- Junior Security Analyst
- Cybersecurity Analyst
- Incident Response Analyst

I will continue updating this repository as I complete additional training, labs, challenges and security investigations.

The purpose of this repository is not simply to record courses completed, but to demonstrate **what I learned, how I understand the concepts, and how those concepts apply to real security investigations**.

---

# 📚 Training Platform

Training completed through **LetsDefend**, a hands-on Blue Team cybersecurity training platform.


**Platform:** LetsDefend  
**Badge:** Network Cable  🏅
**Status:** 🟢 Completed


**Primary Focus:** SOC Operations | Blue Team | Incident Investigation | Malware Analysis | Network Security

#LetsDefend #NetworkCable #Networking #NetworkFundamentals #NetworkSecurity #TCPIP #OSIModel #Subnetting #BlueTeam #SOCAnalyst #Cybersecurity
