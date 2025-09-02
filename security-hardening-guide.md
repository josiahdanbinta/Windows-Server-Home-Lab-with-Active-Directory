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
