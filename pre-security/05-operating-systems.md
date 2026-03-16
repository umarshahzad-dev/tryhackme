# 05 - Operating Systems Basics

The Operating System (OS) is the core software that coordinates everything on a computer, sitting between the user, the applications, and the physical hardware.

---

## 🧠 OS Core Architecture
An OS manages hardware through a series of privilege layers to ensure stability and security.

### Privilege Layers
* **Kernel Space**: The privileged, locked-down core of the OS where the **Kernel** runs. It has unrestricted access to all hardware.
* **User Space**: The area where regular applications run. Apps are prevented from accessing hardware directly and must use **System Calls** to request kernel actions.

```mermaid
graph LR
    A[User Space: Apps] -- System Call --> B[Kernel Space: OS Core]
    B -- Direct Access --> C[Hardware: CPU/RAM]
```



---

## 🛠️ Core Duties of an OS
* **Process Management**: Schedules and prioritizes running programs so the computer doesn't freeze.
* **Memory Management**: Allocates RAM to processes and ensures they don't interfere with each other.
* **File System Management**: Organizes files into directories and manages permissions (Read/Write/Execute).
* **Device Management**: Loads drivers to provide a "Hardware Abstraction Layer" so apps can use devices like mice or printers universally.

---

## 🖥️ Windows vs. Linux CLI
Professionals use the Command-Line Interface (CLI) because it is faster, more precise, and allows for automation.

| Task | Windows (CMD) | Linux (Bash) |
| :--- | :--- | :--- |
| **Current Location** | `cd` | `pwd` |
| **List Files** | `dir` | `ls` |
| **Change Directory** | `cd <folder>` | `cd <folder>` |
| **Read File** | `type <file>` | `cat <file>` |
| **Current User** | `whoami` | `whoami` |
| **Network Config** | `ipconfig` | `ifconfig` or `ip addr` |

---

## 🛡️ Operating System Security
The OS is the first line of defense before any antivirus software.
* **Authentication**: Verifies identity through passwords or biometrics.
* **Permissions**: Implements the **Principle of Least Privilege**, ensuring users only access what they need.
* **Isolation**: Keeps processes in "protected boxes" to prevent a single crash or virus from taking down the entire system.

> [!WARNING]
> **Common Vulnerabilities**:
> **Weak Passwords**: Sequences like `123456` or keyboard patterns like `qwerty` are easily guessed by dictionary attacks.
> **Malware**: Trojan horses and Ransomware exploit weak permissions to encrypt your data for ransom.

---

## 🔗 Original Resources
* [THM Room: OS Introduction](https://tryhackme.com/room/osintroduction)
* [THM Room: Windows Basics](https://tryhackme.com/room/windowsbasics)
* [THM Room: Linux CLI Basics](https://tryhackme.com/room/linuxclibasics)
* [THM Room: Windows CLI Basics](https://tryhackme.com/room/windowsclibasics)
* [THM Room: OS Security](https://tryhackme.com/room/ossecurity)

---
*Next Module: [Software Basics](./06-software-basics.md)*