# packet-tracer-threat-landscape
Cybersecurity investigation lab using Cisco Packet Tracer to analyze network misconfiguration, phishing, rogue access points, and DNS hijacking.
# Cisco Packet Tracer – Investigate a Threat Landscape

## 🔐 Project Overview

This project demonstrates a cybersecurity investigation performed in Cisco Packet Tracer. The objective was to identify vulnerabilities, understand how threat actors could exploit them, and propose appropriate security controls.

The lab focuses on three security scenarios:

* Network configuration vulnerability
* Phishing and malware
* Rogue wireless access point and DNS hijacking

## 🎯 Objectives

* Investigate a misconfigured wireless network.
* Identify security weaknesses that could allow unauthorized access to internal devices.
* Analyze a simulated phishing attack.
* Understand the potential impact of malware on an organization.
* Investigate a rogue wireless access point.
* Analyze how DHCP and DNS can be abused to redirect users to malicious websites.
* Identify appropriate defensive measures.

## 🛠️ Tools & Technologies

* Cisco Packet Tracer
* Nmap
* Wireless networking
* DNS
* DHCP
* IP networking
* Phishing awareness
* Network security
* Threat analysis

## 🔎 Investigation 1 – Network Configuration Vulnerability

The first scenario investigated a vulnerable home wireless network.

A guest wireless network was accessible without authentication and allowed access to devices on the internal network. The investigation demonstrated how an improperly configured guest network could expose internal devices.

### Security Risks Identified

* Unauthorized network access
* Insufficient wireless security
* Guest-to-internal network access
* Exposure of internal devices
* Potential unauthorized access to connected devices

### Recommended Mitigations

* Enable strong wireless encryption.
* Use strong and unique administrator credentials.
* Disable default credentials.
* Isolate guest networks from internal networks.
* Review firewall and router security settings.
* Regularly update network devices.

## 📧 Investigation 2 – Phishing & Malware

The second scenario simulated a phishing attack.

The investigation demonstrated how a malicious email can persuade users to visit a fraudulent website and potentially expose an organization to malware.

### Security Risks

* Credential theft
* Malware infection
* Unauthorized access
* Data loss
* Lateral movement within an organization
* Business disruption

### Recommended Mitigations

* Security awareness training
* Phishing simulations
* Email filtering
* Firewall and intrusion prevention controls
* Malicious URL filtering
* Endpoint protection
* User reporting procedures

## 📡 Investigation 3 – Rogue Access Point & DNS Hijacking

The third scenario investigated a rogue wireless access point.

A threat actor could create a wireless network using a convincing SSID and attempt to attract users into connecting to it.

The scenario also demonstrated how DHCP and DNS services could be manipulated to redirect users toward a malicious server.

### Security Risks

* Man-in-the-middle attacks
* Traffic interception
* Credential exposure
* DNS manipulation
* Malicious website redirection
* Loss of confidentiality

## 🧠 Attack Chain

The simulated attack can be summarized as:

```text
Rogue Wi-Fi
     ↓
Victim connects
     ↓
Attacker-controlled network
     ↓
DHCP provides network configuration
     ↓
Malicious DNS server
     ↓
DNS resolution manipulated
     ↓
Victim redirected to malicious server
```

## 🛡️ Key Security Lessons

This lab reinforced the importance of:

* Network segmentation
* Secure wireless configuration
* Strong authentication
* DNS security
* DHCP security
* Security awareness training
* Endpoint protection
* Continuous monitoring

## 📚 Skills Demonstrated

**Networking**

* IP addressing
* DHCP
* DNS
* Wireless networking
* Network troubleshooting

**Cybersecurity**

* Vulnerability identification
* Threat analysis
* Phishing awareness
* Rogue access point analysis
* DNS hijacking analysis
* Security mitigation

## ⚠️ Disclaimer

This project was performed in a controlled Cisco Packet Tracer lab environment for educational purposes. The phishing scenario was simulated strictly for cybersecurity training.

## 📌 Learning Outcome

This project helped develop practical skills in identifying network vulnerabilities, understanding common attack techniques, analyzing attack paths, and recommending appropriate security controls.
