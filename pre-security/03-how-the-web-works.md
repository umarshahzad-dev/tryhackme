# 03 - How The Web Works

Understanding the web is about understanding the request-response cycle between a client (your browser) and a server.

---

## 🗺️ DNS (Domain Name System)
DNS is the "Phonebook of the Internet," translating human-readable names (tryhackme.com) into machine-readable IP addresses (104.26.10.229).

### The DNS Request Hierarchy
```mermaid
graph TD
    A[Client Request] --> B[Local Cache]
    B -- Not Found --> C[Recursive DNS Server/ISP]
    C -- Not Found --> D[Root Servers]
    D --> E[TLD Servers .com, .org]
    E --> F[Authoritative Nameservers]
    F --> G[A Record Returned]
```

### Common DNS Record Types
* **A Record**: Maps to an IPv4 address.
* **AAAA Record**: Maps to an IPv6 address.
* **CNAME**: An alias; points one domain to another domain.
* **MX Record**: Identifies the servers handling email for the domain.
* **TXT Record**: Holds arbitrary text; often used for security verification (SPF, DKIM).

---

## 🏎️ HTTP & HTTPS
**HTTP** is the set of rules for communicating with web servers. **HTTPS** is the secure version, using SSL/TLS to encrypt data in transit.

### URL Structure
`http://user:password@tryhackme.com:80/view-room?id=1#task3`
1. **Scheme**: `http://`
2. **Host**: `tryhackme.com`
3. **Port**: `:80` (Standard for HTTP)
4. **Path**: `/view-room`
5. **Query String**: `?id=1`
6. **Fragment**: `#task3`

### Common HTTP Methods
* **GET**: Retrieve data from a server.
* **POST**: Send data to a server to create a resource.
* **PUT**: Update an existing resource on the server.
* **DELETE**: Remove a resource.

### HTTP Status Codes
* **200 OK**: Request successful.
* **301/302**: Redirection.
* **401/403**: Unauthorized or Forbidden.
* **404**: Not Found.
* **500/503**: Server-side errors.

---

## 🏗️ How Websites Are Built
Websites consist of two major parts: **The Front End** (Client-side) and **The Back End** (Server-side).

| Technology | Purpose |
| :--- | :--- |
| **HTML** | The structure and skeleton of the page. |
| **CSS** | The styling and visual layout. |
| **JavaScript** | The interactivity and dynamic features. |

> [!CAUTION]
> **Security Context (Web Development)**:
> **Sensitive Data Exposure**: Always check the "View Source" or Developer Tools. Developers often accidentally leave API keys or internal links in HTML comments or JS files.
> **HTML Injection**: Occurs when a site fails to "sanitize" user input. If I can input `<h1>Hacked</h1>` into a form and it displays on the page, the site is vulnerable.

---

## 🛡️ Protecting the Web
* **WAF (Web Application Firewall)**: Sits in front of the server to filter out malicious requests and rate-limit bots.
* **Load Balancer**: Distributes traffic across multiple servers to prevent crashes and ensure high availability.
* **CDN (Content Delivery Network)**: Stores static files (images, JS) on servers worldwide so they load faster for local users.

---

## 🔗 Original Resources
* [THM Room: DNS in Detail](https://tryhackme.com/room/dnsindetail)
* [THM Room: HTTP in Detail](https://tryhackme.com/room/httpindetail)
* [THM Room: How Websites Work](https://tryhackme.com/room/howwebsiteswork)
* [THM Room: Putting It All Together](https://tryhackme.com/room/puttingitalltogether)

---
*Next Module: [Computer Fundamentals](./04-computer-fundamentals.md)*