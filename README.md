
Secure Portable Router Project
==============================

This project, developed at **TEK-UP Private Higher School of Technology and Engineering** , presents the design and implementation of a **secure portable network solution**. It is a modular system built on a Raspberry Pi that addresses modern threats in both personal and public environments by integrating advanced monitoring, traffic filtering, and secure communication.

🌟 Key Features
---------------

*   **Intrusion Detection:** Uses **Snort** to monitor LAN traffic for malicious activity and common attack patterns like port scans or malware signatures.
    
*   **DNS Filtering:** Features **Pi-hole** as a network-wide filter to block ads, malicious domains, and unwanted content for all connected devices.
    
*   **Honeypot Integration:** Implements **Cowrie**, a high-interaction SSH and Telnet honeypot, to capture attacker activity and analyze malicious behavior.
    
*   **Secure Internet Access:** Uses **OpenVPN** to route all outbound traffic through encrypted tunnels, ensuring privacy and protection against eavesdropping in untrusted environments (e.g., public Wi-Fi).
    
*   **Network Segmentation:** Leverages firewalls and routing to isolate critical components and separate LAN, WAN, and secure VPN connections.
    
*   **Portability:** Designed to be compact and mobile, allowing for easy deployment in diverse scenarios.
    

🛠 Tech Stack
-------------

### Hardware

*   **Main Unit:** Raspberry Pi 4 (4 GB RAM, 32 GB SD Card).
    
*   **Network Interfaces:** Built-in Ethernet and optional USB Wi-Fi adapters for WAN connectivity.
    

### Software

*   **Core OS:** **OpenWRT** – A lightweight and flexible Linux operating system for embedded devices.
    
*   **Security Tools:** Snort (IDS/IPS), Pi-hole (DNS filter), Cowrie (Honeypot), and OpenVPN (Encryption).
    
*   **Environment:** Docker (used for containerized deployment of security services).
    

🚀 Implementation Overview
--------------------------

### 1\. Core Operating System

Flash the Raspberry Pi with **OpenWRT**, configure the LAN/WAN interfaces, and set up firewall zones to segment internal and external traffic.

### 2\. Intrusion Detection

Deploy **Snort** to capture LAN traffic and apply rule sets for real-time threat detection and logging.

### 3\. Traffic Filtering

Deploy **Pi-hole** (typically in a container) and configure it as the primary DNS server for the network to enforce domain-based filtering.

### 4\. Active Defense

Set up **Cowrie** to emulate vulnerable services (SSH/Telnet), allowing for the observation and logging of attacker interactions.

### 5\. Encrypted Tunneling

Configure **OpenVPN** to ensure that all data leaving the router remains confidential and anonymous.

📂 Project Structure
--------------------

*   /docs: Contains the full technical report and architecture diagrams.
    
*   /Pics: Contains prove of work ( Screenshots for resaults)

-------------------------- 

**Author:** Saii Nassim

**Academic Year:** 2025-2026

**Institution:** TEK-UP University, Tunisia
