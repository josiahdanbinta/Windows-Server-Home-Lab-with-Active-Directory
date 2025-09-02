# 🖥️ Windows Server Home Lab with Active Directory

## Objective
Build a secure Windows Server 2022 Home Lab with **Active Directory**, **DNS**, and **DHCP** for hands-on cybersecurity learning and enterprise environment simulation.

---

## Lab Goals
- Install and configure **Windows Server 2022** in a virtualized environment.
- Set up **Active Directory Domain Services (AD DS)**.
- Configure **DNS** and **DHCP** for network management.
- Create and manage **users, groups, and organizational units (OUs)**.
- Apply **Group Policy Objects (GPOs)** for security hardening.

---

## Lab Setup

### 1. Environment
- **Virtualization Software:** VirtualBox / VMware Workstation
- **VMs:**  
  - Windows Server 2022 (Domain Controller)  
  - Windows 10/11 (Client Machines)

### 2. Installation Steps
1. Install **Windows Server 2022** on VM.
2. Configure network adapter (Host-Only / Internal Network).
3. Install **Active Directory Domain Services** via Server Manager.
4. Promote the server to a **Domain Controller**.
5. Configure **DNS** and **DHCP** roles.
6. Create test **users, groups, and OUs**.
7. Apply **GPOs** for password policy, desktop restrictions, and audit logging.

---

## Network Diagram
![AD Home Lab Diagram](ad-home-lab-diagram.png)

---

## Skills Demonstrated
- Windows Server Administration
- Active Directory Management
- DNS & DHCP Configuration
- Group Policy Implementation
- Network Diagramming
- Security Hardening

---
# 🔐 Security Hardening Guide – Windows Server & Security Onion Lab

## 1. Introduction
This guide details the security measures implemented in the Windows Server Home Lab with Active Directory and Security Onion.  
It focuses on reducing attack surfaces, improving detection, and increasing resilience against threats.

---

## 2. Operating System Hardening
- ✅ Install the latest Windows Server & Windows 10 updates.
- ✅ Remove unused roles, features, and services.
- ✅ Disable SMBv1 and enforce SMB signing.
- ✅ Configure Windows Defender with real-time protection.

---

## 3. Active Directory Security
- Enforce **strong password policies** (length, complexity, expiration).
- Enable **Account Lockout Policies** to block brute-force attempts.
- Use **Privileged Access Workstations (PAWs)** for admin tasks.
- Audit and monitor logon events.

---

## 4. Network Security
- Segment the lab network (VLANs for clients, servers, and monitoring).
- Block unnecessary inbound and outbound ports in the firewall.
- Restrict RDP to trusted IP ranges.
- Enable IPS mode in Security Onion.

---

## 5. Security Onion Configuration
- Update rule sets (ET Open, Proofpoint).
- Tune Suricata and Zeek to reduce false positives.
- Configure alert forwarding to SIEM.
- Enable file extraction and hash calculation.

---

## 6. User Awareness
- Conduct phishing simulations using GoPhish.
- Provide basic security awareness training to test users.
- Encourage reporting of suspicious emails.

---

## 7. Backup & Recovery
- Configure regular backups for AD and DNS databases.
- Test recovery procedures quarterly.
- Store offline copies of critical backups.

---

## 8. Continuous Improvement
- Monthly vulnerability scans with OpenVAS.
- Review Security Onion logs weekly.
- Update Group Policy settings as new threats emerge.

---

## 9. Lessons Learned
- Layered security reduces impact of incidents.
- Continuous monitoring detects issues early.
- Human factors remain a major risk — training is critical.

---
