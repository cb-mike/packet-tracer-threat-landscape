# Packet-tracer-threat-landscape
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
* Security mitigation.

# SCREENSHOOTS
## Network-topology.png

<img width="550" height="502" alt="topology" src="https://github.com/user-attachments/assets/68751399-9773-4419-a92b-e4504544aa39" />

<img width="1078" height="667" alt="home-cafe-isp-workoffices" src="https://github.com/user-attachments/assets/2b2bc0e2-7897-48bf-90e3-f699ddaa889a" />


## Vulnerable-wireless-network.png

<img width="827" height="452" alt="credentials" src="https://github.com/user-attachments/assets/dff12b1b-6b99-4ba3-9e8a-5b3d544543a2" />

<img width="808" height="862" alt="security risk1" src="https://github.com/user-attachments/assets/11935b62-59a0-42fb-b309-841bb145f2b9" />

<img width="816" height="803" alt="security riskk 2" src="https://github.com/user-attachments/assets/2bd188a9-5333-43d5-a42b-7c7287b365f7" />


## Phishing-scenario.png

<img width="852" height="577" alt="phishing email from HACKER" src="https://github.com/user-attachments/assets/bf222a27-f82e-4e79-ab2e-74639ead89f4" />

<img width="851" height="598" alt="phishing email at victim" src="https://github.com/user-attachments/assets/415d1c5b-ea75-4be7-8437-14840175adf1" />

<img width="828" height="408" alt="web-victim" src="https://github.com/user-attachments/assets/fe5c0a1d-be13-42af-a669-8e9be5d38f16" />

<img width="850" height="616" alt="infected Victim" src="https://github.com/user-attachments/assets/31abcd2c-c7a6-4501-81ed-77340718f9d3" />

## Rogue-access-point.png

<img width="647" height="537" alt="threat actor´s bag" src="https://github.com/user-attachments/assets/d68a3800-4fc4-4871-8675-e4b0c585870f" />

<img width="632" height="570" alt="public wifi" src="https://github.com/user-attachments/assets/e17010ac-8250-4c59-9e5d-845892933e90" />

<img width="845" height="566" alt="victim social website" src="https://github.com/user-attachments/assets/b1323f23-5dfb-42c4-b5ed-253971cb4fca" />

<img width="850" height="566" alt="victim hacked" src="https://github.com/user-attachments/assets/e8fe0350-774a-400f-b37c-2d01ec7e9b8c" />

## dns-hijacking.png

The host IP addres
ses are different, but this is normal. Each host on a LAN needs a unique IP address. The subnet masks are the same. The DNS server addresses are different.

<img width="1261" height="506" alt="two laptops in cafe" src="https://github.com/user-attachments/assets/d925b690-9d3a-4e28-94fd-938ea0d7fda9" />


When Cafe Customer connected to the rogue access point's wireless network, it received an IP address configuration from DHCP. The DHCP server is configured to distribute the hacker laptop address as the DNS server address. The DNS server on the Cafe Hacker Laptop associates the IP address of a malicious server, 10.6.0.250, with the name of a popular website, friends.example.com. When the user of the Cafe Customer laptop tries to visit the website, traffic is redirected to the malicious server instead. Ransomware is then installed on Cafe Customer laptop the user's files are encrypted.

<img width="1823" height="501" alt="comparison " src="https://github.com/user-attachments/assets/33e36090-6062-4503-a806-d5558f01211b" />

<img width="837" height="537" alt="threat actor´s server" src="https://github.com/user-attachments/assets/7b5acf44-f74a-4d58-a174-d3d280cff6ab" />

<img width="847" height="582" alt="DHCP" src="https://github.com/user-attachments/assets/77a4d86f-63d2-44f4-8ac6-1d295e1f4eaa" />

## ⚠️ Disclaimer

This project was performed in a controlled Cisco Packet Tracer lab environment for educational purposes. The phishing scenario was simulated strictly for cybersecurity training.

## 📌 Learning Outcome

This project helped me develop practical skills in identifying network vulnerabilities, understanding common attack techniques, analyzing attack paths, and recommending appropriate security controls.
