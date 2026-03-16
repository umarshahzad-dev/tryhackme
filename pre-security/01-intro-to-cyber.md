# 01 - Introduction to Cyber Security

This module serves as the foundational entry point into the cybersecurity mindset, covering the fundamental distinction between offensive and defensive operations and the career paths available within the industry.

---

## 🚩 Offensive Security (Ethical Hacking)
**Definition**: The practice of breaking into systems, exploiting vulnerabilities, and finding loopholes to understand attacker methods and improve defenses.

> [!IMPORTANT]
> **Core Mindset**: To outsmart a hacker, you must think like one. This involves experimenting in controlled environments and documenting findings to proactively close security gaps.

### Directory Brute-Forcing
A methodology used to discover hidden files or directories on a web server by guessing names based on common developer patterns (e.g., `/admin`, `/backup`, `/config`).

#### Tool Focus: `dirb`
* **Purpose**: Discovers hidden web content by sending HTTP requests based on a wordlist.
* **Standard Wordlist**: `/usr/share/dirb/wordlists/common.txt`
* **Key Output**: 
    * `CODE: 200` (Success/Found)
    * `CODE: 301` (Redirect)

---

## 🛡️ Defensive Security (Blue Teaming)
**Definition**: The practice of protecting networks, systems, and data through continuous monitoring, detection, and incident response.

### Core Pillars of Defense
1.  **Monitoring & Detection**: Identifying suspicious behavior (e.g., "impossible travel" logins).
2.  **Incident Response**: Containing and removing active threats.
3.  **Threat Intelligence**: Proactive defense based on gathering data on attacker trends.
4.  **Vulnerability Management**: Identifying and prioritizing the patching of system flaws.

### Strategy: Defense in Depth
The concept of using multiple layers of security controls so that if one fails, others remain to provide protection.

| Layer | Security Control | Purpose |
| :--- | :--- | :--- |
| **Human** | Employee Training | Creating a "Human Firewall" against phishing. |
| **Network** | Firewalls / IDS | Filtering traffic and monitoring for anomalies. |
| **Policy** | Security Policies | Enforcing strong passwords and usage rules. |

---

## 🏗️ Security Operations & Infrastructure
### SOC (Security Operations Centre)
A centralized, 24/7 team responsible for reviewing alerts and responding to incidents in real-time.

### SIEM (Security Information & Event Management)
A centralized system that aggregates and analyzes data from across an entire IT infrastructure.
> **Analogy**: SIEM is like a "digital radar" sweeping the environment to find disconnected data points and turn them into actionable alerts.

---

## 💼 Cyber Security Career Paths
| Role | Primary Focus | Learning Path |
| :--- | :--- | :--- |
| **Security Analyst** | Evaluates networks and recommends preventative measures. | SOC Level 1 |
| **Security Engineer** | Designs and maintains security controls/networks. | Jr. Pentester |
| **Incident Responder** | Mitigates attacks as they unfold in real-time. | SOC Level 1 |
| **Malware Analyst** | Reverse-engineers malicious code (Asm, C). | Advanced |
| **Penetration Tester** | Legally hacks systems to find loopholes. | Offensive Pentesting |

> [!NOTE]
> **Security Context (Programming)**:
> Malware analysis requires low-level programming knowledge (Assembly/C) to understand how compiled programs interact with CPU and Memory in a "de-compiled" state.

---

## 🔗 Original Resources
* [THM Room: Offensive Security Intro](https://tryhackme.com/room/offensivesecurityintro)
* [THM Room: Defensive Security Intro](https://tryhackme.com/room/defensivesecurityintro)
* [THM Room: Careers in Cyber](https://tryhackme.com/room/careersincyber)

---
*Next Module: [Network Fundamentals](./02-network-fundamentals.md)*