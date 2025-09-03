# Albion University Network Design and Implementation

## 📌 Project Overview
This project involves the planning, design, and configuration of a **scalable university network topology** for Albion University using **Cisco Packet Tracer**. The goal is to ensure secure, reliable, and efficient communication between different departments, campuses, and external services.

The network is designed to meet the university’s academic and administrative requirements while supporting **VLAN segmentation, dynamic addressing, and RIP routing** for inter-campus communication.

---
<img width="1662" height="614" alt="Screenshot 2025-09-03 151849" src="https://github.com/user-attachments/assets/66afb3a4-4aa5-41a9-892b-aed4fd57d818" />

## 🏫 Network Requirements
- **Main Campus:**
  - **Building A**: Administrative staff (HR, Finance, Management) and Business Faculty (VLAN segmentation expected).
  - **Building B**: Faculty of Engineering, Computing, and Arts & Design.
  - **Building C**: Student labs and IT department (hosts web server and other servers).
- **Smaller Campus:**
  - Faculty of Health and Sciences (separate VLANs for staff and students).
- **External Cloud**:
  - Email server hosted outside the university.

---

## ⚙️ Key Features & Configurations
- **VLANs** for departmental segmentation:
  - VLAN10 → Finance (192.168.1.0/24)
  - VLAN20 → Management (192.168.2.0/24)
  - VLAN30 → Business (192.168.3.0/24)
  - VLAN40 → Engineering & Arts (192.168.4.0/24, 192.168.5.0/24)
  - VLAN60 → IT Department (192.168.6.0/24)
  - VLAN70 → Students (192.168.7.0/24)
  - VLAN80 → Web Server (192.168.8.0/24)
  - VLAN90 → Health Science Staff (192.168.10.0/24)
  - VLAN100 → Health Science Students (192.168.9.0/24)
- **RIPv2** for dynamic routing across routers.
- **DHCP** (router-based) to assign dynamic IPs to end devices.
- **Servers**:
  - Internal **Web Server** hosted in Building C (IT).
  - External **Email Server** hosted in the cloud.
- **Security**: VLAN segmentation, ACLs (Access Control Lists), and switch security configurations.

---

## 🖥️ Tools & Technologies
- Cisco Packet Tracer (network simulation)
- VLANs & Inter-VLAN Routing
- RIP Version 2 (Dynamic Routing Protocol)
- DHCP Services
- Network Security (Switchport security, ACLs)

---

## 📊 Topology Diagram
The network is designed with hierarchical architecture:
- **Core Router** connects main campus, small campus, and external cloud.
- **Distribution Layer Switches** manage departmental VLANs.
- **Access Layer Switches** connect PCs, printers, and servers.

(📌 *See attached Packet Tracer topology diagram*).

---

## ✅ Outcomes
- Seamless connectivity between **two campuses** and the **cloud-hosted email server**.
- Secure departmental isolation via **VLANs**.
- Centralized DHCP for automated IP allocation.
- Dynamic routing with **RIPv2** ensures scalable inter-campus communication.
- Internal and external server access configured successfully.

---

## 🚀 How to Use
1. Open the `.pkt` file in Cisco Packet Tracer.
2. Start simulation and verify:
   - PC-to-PC communication within VLANs.
   - Inter-VLAN communication via router-on-a-stick.
   - External email server reachability.
3. Test DHCP IP allocation and RIP routing.

---

## 📄 Report (Academic Requirement)
A detailed report (max 1500 words) has been prepared including:
- Network design justification
- Performance evaluation
- Scalability, reliability, and security analysis

---

## 👤 Author
**Sachin Rana**  
- 💻 Networking & Cloud Enthusiast  
- 🔗 [GitHub Profile](#) | [LinkedIn Profile](#)  
