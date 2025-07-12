# Linux Networking Basics

In this README, you will find a summarized version of key Linux networking concepts.

---

## Table of Contents

1. Local Area Network (LAN)
2. IP Addresses and Subnets
3. Switches and Routers
4. Gateway and NAT
5. Firewall and Ports
6. DNS (Domain Name System)
7. Networking Commands

---

## 1. Local Area Network (LAN)

- A LAN connects multiple devices (e.g., phones, computers, printers) within a physical location.
- Each device is uniquely identified using an **IP address**.

---

## 2. IP Address and Subnet

- IP address: 32-bit value represented in four octets (e.g., 192.168.0.1).
- Subnet mask determines which portion of the IP is the **network** and which is the **host**.
- Example:
  - Subnet: `255.255.255.0` (24 fixed bits)
  - IP Range: `192.168.0.1` to `192.168.0.255`
- CIDR notation: `192.168.0.0/24`

---

## 3. Switches and Routers

- **Switch:** Forwards traffic within LAN based on IP addresses.
- **Router:** Connects LAN to WAN (Internet) and performs **Network Address Translation (NAT)**.

---

## 4. Gateway and NAT

- **Gateway:** Router’s IP in the LAN, used to access external networks.
- **NAT:** Translates internal LAN IP to external public IP (used for Internet communication).

---

## 5. Firewall and Ports

- **Firewall:** Set of rules that control inbound/outbound traffic.
- **Ports:** Logical access points on a device for network services.
  - Port 80 → HTTP
  - Port 443 → HTTPS
  - Port 3306 → MySQL
  - Port 5432 → PostgreSQL

---

## 6. DNS (Domain Name System)

- Resolves human-readable names (e.g., `facebook.com`) to IP addresses.
- Structure: Root → TLD (.com, .org, .edu) → Domain name (devops.com) → Subdomain (tutorial.devops.com)
- Managed by ICANN.
- Common TLDs:
  - `.com`, `.org`, `.edu`, `.gov`, `.mil`, `.net`
  - Country code TLDs: `.uk`, `.us`, `.de`, etc.
- DNS resolution translates human-readable domain names (like https://www.google.com/search?q=google.com) into machine-readable IP addresses (like 172.217.160.142). This process allows your computer to locate and connect to the correct server on the internet.

---

## 7. Useful Networking Commands

![Linux Network](Images/network.gif)

| Command    | Description                               |
| ---------- | ----------------------------------------- |
| `ifconfig` | Shows network interfaces and IP addresses |
| `netstat`  | Lists active ports and connections        |
| `ps aux`   | Lists running processes                   |
| `nslookup` | Queries DNS for domain to IP (or reverse) |
| `ping`     | Checks connectivity to an IP or domain    |

---

## Summary

As a DevOps engineer, understanding:

- IP addressing and subnetting
- DNS resolution
- Firewall/port configuration
- Basic network tools

...is essential to configure and troubleshoot Linux servers effectively.

🧑‍💻 _Created by Rico John Dato-on_  
🔗 [LinkedIn](https://www.linkedin.com/in/rico-john-dato-on) • [Portfolio](https://ricodatoon.netlify.app)
