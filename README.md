# 🛡️ Cybersecurity Detection & Monitoring Homelab


![image](https://github.com/user-attachments/assets/c40364ea-602c-476b-8815-94e4826354d7)



## 👋 Welcome!

Hi, I’m Manny—a curious hacker, passionate learner, and junior cybersecurity processional starting my journey in the field.

This homelab is where I practice detection, monitoring, threat hunting, and defensive blue team techniques. Inspired by the [CyberWox Homelab](https://cyberwoxacademy.com/building-a-cybersecurity-homelab-for-detection-monitoring/), I built this environment to gain real-world, hands-on experience with professional-grade tools and technologies. 

It’s a space for me to experiment, break things (ethically 😉), and sharpen the skills that will carry me into the field.

I built this lab to:
- Hone my ethical hacking skills ⚔️  
- Practice blue team detection & incident response 🛡️  
- Learn and configure open-source security tools 🔧  
- Monitor attacks using enterprise-grade setups 📊  

---

## 🧠 Skills Demonstrated

✅ Network segmentation & VM provisioning  
✅ Firewall configuration using **pfSense**  
✅ Attack simulation with **Kali Linux**  
✅ SIEM setup using **Splunk** & **Universal Forwarder**  
✅ Network monitoring with **Security Onion**  
✅ Log collection & forwarding  
✅ Active Directory domain setup  
✅ Custom VLAN creation in VMware  

---

## 🧰 Tools & Technologies

| Role              | Tool / OS                        | IP Address        |
|-------------------|----------------------------------|-------------------|
| Attacker          | Kali Linux                       | `192.168.1.1` (em1) |
| Firewall          | pfSense                          | `192.168.***.***` (router) |
| Monitoring        | Security Onion                   | `192.168.3.1` (em3) |
| SIEM              | Splunk + Universal Forwarder     | `192.168.4.1` (em5) |
| Victim Machines   | Windows 10                       | `192.168.2.1` (em2) |
| Domain Controller | Windows Server (AD)              | `192.168.2.1` (em2) |

---

## 🔍 Network Overview

- **VMware Virtual Networks** (VMnet2 - VMnet6) are used to isolate traffic and segment network layers.
- **pfSense** firewall routes and inspects traffic between attacker and victim networks.
- **SPAN port** on `em4` allows **Security Onion** to sniff mirrored traffic for IDS analysis.
- **Splunk** ingests logs from victims and the domain controller via **Universal Forwarder**.
- This architecture allows simulation of APT-style attacks and Blue Team monitoring.

---

## ⚔️ Offensive Testing

With **Kali Linux**, I plan to conduct:

- Network discovery with `nmap`, `netdiscover`, `arp-scan`
- Credential attacks with `hydra`, `medusa`
- Exploits using `Metasploit`, `searchsploit`, `msfvenom`
- Web application fuzzing using `Burp Suite`, `Gobuster`, `Nikto`
- Lateral movement and privilege escalation in Active Directory

---

## 🛡️ Defensive Analysis

Using **Security Onion** and **Splunk**, I will practice:

- Detecting brute force, port scanning, and malware activity  
- Parsing and analyzing logs from Linux/Windows victims  
- Using `Zeek`, `Suricata`, `Wazuh`, and `Sysmon` for alerts  
- Writing basic Sigma rules for detection use cases  
- Creating dashboards and visualizations in Splunk  

---

## 🎯 Goal
This project is part of my transition into the cybersecurity field, where I’m actively building the skills needed to break into the industry. My immediate goal is to land a SOC Analyst role and eventually grow into Threat Hunting or Red Team work.

This homelab reflects my curiosity, dedication, and passion for learning through hands-on experience. It's not just a project—it’s a stepping stone toward where I want to be.

---



