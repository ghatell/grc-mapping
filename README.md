# 📑 GRC Mapping – Incident Response & Compliance

This section follows the [Incident Handling & Analysis Project](https://github.com/ghatell/incident-handling-analysis) and maps each incident scenario to relevant controls from **NIST SP 800-53** and **ISO/IEC 27001**. It demonstrates how technical incident handling aligns with governance, risk, and compliance standards — a key capability in GRC roles.

---

## 📊 Incident #1 – DDoS Attack (ICMP Flood)

### 🔐 NIST 800-53 Mapping

| **Control** | **Description** | **Application** |
|------------|------------------|-----------------|
| `SC-5` | Denial of Service Protection | Firewall rules limited ICMP traffic rate to reduce DDoS impact. |
| `SI-4` | System Monitoring | Network monitoring tools were deployed to detect abnormal traffic. |
| `IR-4` | Incident Handling | Team followed response procedures and log analysis post-event. |
| `CP-10` | System Recovery | Prioritized restoration of critical network services. |

### 📘 ISO/IEC 27001 Mapping

| **Clause / Control** | **Description** | **Application** |
|----------------------|------------------|-----------------|
| `A.12.1.3` | Capacity Management | Prioritized service restoration for availability during attack. |
| `A.16.1.1` | Incident Response Policies | Response was structured and documented. |
| `A.16.1.4` | Classification of Incidents | ICMP flood was analyzed and responded to accordingly. |
| `A.17.1.2` | Continuity Measures | Ensured systems were brought back online in a secure sequence. |

---

## 📊 Incident #2 – Phishing & Data Breach

### 🔐 NIST 800-53 Mapping

| **Control** | **Description** | **Application** |
|------------|------------------|-----------------|
| `IA-2` | Identification & Authentication | MFA and login limits were enforced post-incident. |
| `AC-2` | Account Management | Compromised intern account was disabled promptly. |
| `AT-2` | Security Awareness Training | Users received phishing awareness training. |
| `IR-6` | Incident Reporting | Incident reported to stakeholders and legal authorities. |
| `CP-9` | Backup and Recovery | Database restored from full backup. |

### 📘 ISO/IEC 27001 Mapping

| **Clause / Control** | **Description** | **Application** |
|----------------------|------------------|-----------------|
| `A.9.2.2` | User Access Provisioning | Intern had excessive access; policy gaps identified. |
| `A.9.4.2` | Secure Log-on | MFA and access restrictions introduced. |
| `A.10.1.1` | Encryption Controls | Encryption was noted as a needed control for data protection. |
| `A.16.1.5` | Breach Notification | Customers and legal were informed of the incident. |
| `A.17.1.3` | Recovery Procedures | Data restored and staff instructed to re-enter missing records. |

---

## ✅ GRC Recommendations

- **Access Reviews**  
  Review account privileges regularly to prevent over-permissioned users.  
  *Controls: `AC-2`, `A.9.2.2`*

- **Formalize & Test IRP**  
  Ensure incident response plans are updated and tested across teams.  
  *Controls: `IR-8`, `A.16.1.1`*

- **Improve Backups & Recovery Testing**  
  Ensure backups are tested for integrity and restore capability.  
  *Controls: `CP-9`, `A.17.1.3`*

- **Phishing Simulations**  
  Conduct mock phishing campaigns and reinforce credential safety.  
  *Controls: `AT-2`, `A.7.2.2`*

---

> 📂 This GRC mapping supports a broader understanding of how technical incidents align with compliance frameworks
