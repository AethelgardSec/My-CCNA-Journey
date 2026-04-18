
#  Cisco CCNA 200-301: Journey to Network Engineering
### *A Comprehensive Study Journal & Technical Documentation*

Welcome to my CCNA study repository! As a high school student passionate about networking and cybersecurity, I am documenting my journey through the **Jeremy's IT Lab CCNA 200-301 Course**. This repository serves as both a personal knowledge base and a showcase of my technical understanding of modern networking architectures.

---

##  Day 1: Introduction to Networking
*Foundational concepts of how data moves across digital landscapes.*

### **Core Definitions**
A **Network** is more than just connected computers; it is a digital ecosystem allowing nodes to share resources. Whether it's two PCs connected by a single cable or the global Internet, the principles remain the same.

### **Network Components**
*   **End Hosts (Endpoints):** The source and destination of data.
    *   **Clients:** Devices requesting services (e.g., my laptop requesting a webpage).
    *   **Servers:** Devices providing services (e.g., a web server hosting this content).
*   **Intermediary Devices:** The "traffic police" of the network.
    *   **Switches:** High-density devices (24/48 ports) that facilitate communication **within** a Local Area Network (LAN).
    *   **Routers:** The gateways that connect different LANs and provide access to the **Internet**.
    *   **Firewalls:** Security sentinels (Hardware or Software) that filter traffic based on defined security postures.

> **Key Insight:** Switching happens *inside* the LAN; Routing happens *between* LANs.
<img width="660" height="800" alt="image" src="https://github.com/user-attachments/assets/a2614235-093f-4890-aab7-feb4114ff7a0" />

---

## 🔌 Day 2: Interfaces and Cables
*The Physical Layer: Understanding the medium of transmission.*

### **1. Data Measurement & Speed**
Precision in measurement is vital for network performance analysis:
*   **Bit (b):** The fundamental unit (0 or 1).
*   **Byte (B):** 8 bits (used for storage).
*   **Bandwidth:** Measured in **bits per second (bps)**.
    *   *Standard:* 1 Gbps = 1,000,000,000 bits per second.

### **2. Copper vs. Fiber-Optic**
| Feature | UTP (Copper/RJ-45) | Fiber-Optic (SFP) |
| :--- | :--- | :--- |
| **Medium** | Electrical signals over copper | Light pulses over glass |
| **Distance** | Max 100m (Standard) | Up to 30km+ (Single-mode) |
| **EMI** | Vulnerable to interference | Immune to EMI |
| **Use Case** | Desktop/LAN connectivity | Backbone/Long-distance links |

### **3. Smart Connectivity: Auto MDI-X**
Historically, we needed **Straight-through** cables for different devices and **Crossover** cables for similar ones. Modern networking utilizes **Auto MDI-X**, which automatically detects and configures the required pinout, reducing physical layer deployment errors.
<img width="394" height="203" alt="スクリーンショット 2026-04-18 071859" src="https://github.com/user-attachments/assets/a7550b29-6c4f-4eeb-8135-687b36347d4e" />
<img width="629" height="279" alt="スクリーンショット 2026-04-18 072117" src="https://github.com/user-attachments/assets/e69c881a-ef64-44f0-8bf8-1cd1a0d3f391" />
<img width="583" height="312" alt="image" src="https://github.com/user-attachments/assets/be24d7a5-328c-461e-87c0-10b5783a5be6" />

---

## 🏗 Day 3: The TCP/IP Model
*The Architectural Blueprint of the Internet.*

### **The 5-Layer Stack**
Understanding the modularity of networking through the TCP/IP model:

1.  **Application (L5):** Where the user interacts (HTTP, DNS, SMTP).
2.  **Transport (L4):** Process-to-process delivery using **Port Numbers**.
    *   *TCP:* Reliable, connection-oriented.
    *   *UDP:* Fast, connectionless.
3.  **Network (L3):** End-to-end delivery across networks using **IP Addresses** (IPv4/IPv6).
4.  **Data Link (L2):** Hop-to-hop delivery within a LAN using **MAC Addresses**.
5.  **Physical (L1):** The actual transmission of bits over the medium.
<img width="710" height="531" alt="image" src="https://github.com/user-attachments/assets/6e685e8a-7d30-47b9-b748-e3a2ac14e52e" />

### **Encapsulation: The "Russian Doll" of Data**
As data travels down the stack, each layer adds its own header (and a trailer at L2). This process is called **Encapsulation**.
*   **L4 PDU:** Segment (TCP) / Datagram (UDP)
*   **L3 PDU:** Packet
*   **L2 PDU:** Frame
*   **L1 PDU:** Bits
<img width="713" height="541" alt="image" src="https://github.com/user-attachments/assets/4dcab50a-b6bd-4a10-b396-8460ead6d04d" />

---
*“The best way to predict the future is to create it.” – This repository is my first step toward becoming a Network Engineer.*
