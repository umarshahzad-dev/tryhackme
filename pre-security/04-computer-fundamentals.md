# 04 - Computer Fundamentals

Understanding the physical and virtual "building blocks" of a computer system is essential for securing the environment and optimizing application performance.

---

## 🏗️ Inside a Computer System
A computer is a collection of components working in unison, managed by firmware and the Operating System.

### The Boot Process
1. **Power On**: PSU sends power to components.
2. **Firmware (UEFI/BIOS)**: Central system managing startup; initializes hardware.
3. **POST (Power-On Self Test)**: Verifies all required components are functioning.
4. **Boot Device Selection**: UEFI searches for the bootup routine (OS location).
5. **Bootloader**: Transfers the OS from storage into RAM and hands over control.

---

## 💻 Computer Types & Trade-offs
Not all computers are designed for human interaction; many are "hidden" or specialized for specific roles.

| Type | Characteristics | Primary Use Case |
| :--- | :--- | :--- |
| **Server** | No screen; high reliability; runs continuously. | Hosting web apps, databases. |
| **Workstation** | Precision and reliability for professional tasks. | 3D modeling, simulations. |
| **IoT Device** | Single-purpose; network-connected. | Smart thermostats, doorbells. |
| **Embedded** | Built into larger machines; often no network. | Car controllers, coffee makers. |

---

## 🤝 Client-Server Model
The foundation of the modern internet, where devices specialize in either requesting or providing services.



[Image of Client-Server Model diagram]


* **Client**: Initiates the request (e.g., your web browser).
* **Server**: Processes the request and serves the resource.
* **Protocol**: The set of rules defining the communication (e.g., HTTP).

---

## ☁️ Virtualization & Cloud Computing
Virtualization allows one physical server to act as multiple separate computers, drastically increasing efficiency.

### Virtual Machines (VMs) vs. Containers
* **Virtual Machine**: A complete virtual computer with its own Operating System. Uses a **Hypervisor** to manage resources.
* **Container**: Lightweight; shares the host's OS kernel to run a single application. Example: **Docker**.

### Cloud Service Models
* **IaaS (Infrastructure)**: You rent the virtual "hardware"; you manage the OS.
* **PaaS (Platform)**: Provider manages the OS; you just upload your code.
* **SaaS (Software)**: Everything is managed by the provider; you just use the app (e.g., Gmail).

---

## 🔗 Original Resources
* [THM Room: Inside a Computer System](https://tryhackme.com/room/insideacomputersystem)
* [THM Room: Computer Types](https://tryhackme.com/room/computertypes)
* [THM Room: Client-Server Basics](https://tryhackme.com/room/clientservertbasics)
* [THM Room: Virtualization Basics](https://tryhackme.com/room/virtualizationbasics)
* [THM Room: Cloud Computing Fundamentals](https://tryhackme.com/room/cloudcomputingfundamentals)

---
*Next Module: [Operating Systems Basics](./05-operating-systems.md)*