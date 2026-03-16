# 07 - Attacks and Defenses

Cybersecurity is the practice of protecting the "CIA Triad"—the three core principles that ensure data is kept secret, accurate, and available.

---

## ⚖️ The CIA Triad
Every security control or attack can be mapped back to these three pillars:

* **Confidentiality**: Ensuring sensitive data is only accessible to authorized individuals.
* **Integrity**: Ensuring data is not modified or tampered with by unauthorized parties.
* **Availability**: Ensuring systems and data are accessible to authorized users when needed.



---

## 🔐 Cryptography Concepts
Cryptography uses mathematical algorithms and secret keys to protect the CIA Triad in transit and at rest.

### Symmetric vs. Asymmetric Encryption
* **Symmetric Encryption**: Uses the same secret key for both encryption and decryption. It is fast but suffers from the "Key Distribution Problem" (how to share the key safely).
* **Asymmetric Encryption**: Uses a **Public Key** (for encryption) and a **Private Key** (for decryption). This solves the key sharing issue because the public key can be openly distributed.

### Digital Certificates & HTTPS
Modern web security uses a hybrid approach:
1.  **Asymmetric Encryption** is used to securely exchange a secret key.
2.  **Symmetric Encryption** then takes over for fast, bulk data transfer during the session.
* **Certificates**: Digital documents signed by a **Certificate Authority (CA)** that prove a public key belongs to a specific entity.

---

## ⚔️ Offensive Security (The Red Team)
Offensive security involves proactively seeking out vulnerabilities to fix them before a malicious actor finds them.

* **Vulnerability**: A weakness or flaw in a system.
* **Exploit**: The method used to take advantage of that weakness.
* **Enumeration**: The process of gathering as much information as possible about a target.
* **Dictionary Attack**: Using a wordlist to guess credentials or hidden directories.

> [!TIP]
> **Hacker Mindset**: Attackers look for the "domino effect." A hidden login page combined with a weak password can lead to a full system compromise.

---

## 🛡️ Defensive Security (The Blue Team)
Defensive security focuses on visibility, prevention, and response.

| Phase | Action |
| :--- | :--- |
| **Prevention** | Implementing firewalls, antivirus, and patches to stop attacks. |
| **Detection** | Monitoring logs and alerts to find suspicious activity. |
| **Mitigation** | Isolating systems or blocking IPs during an active incident. |
| **Analysis** | Investigating the "Who, What, and How" after an incident occurs. |



---

## 🔗 Original Resources
* [THM Room: The CIA Triad](https://tryhackme.com/room/theciatriad)
* [THM Room: Cryptography Concepts](https://tryhackme.com/room/cryptographyconcepts)
* [THM Room: Become a Hacker](https://tryhackme.com/room/becomeahacker)
* [THM Room: Become a Defender](https://tryhackme.com/room/becomeadefender)

---
*Back to [Path Overview](./README.md)*