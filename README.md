# Cybersecurity-Incident-Response-Simulation
Virtual Incident Response Plan and Post-Incident Analysis for YuvaIntern Week 2
# Virtual Security Incident Response Simulation

##  Project Overview:
This repository contains the Incident Response Plan and Post-Incident Analysis for a simulated security breach. The objective of this project is to analyze a security incident, contain and eradicate the threat, and restore normal operations following standard cybersecurity frameworks.

---

##  Framework Used:
* **NIST SP 800-61 Rev. 2** (Computer Security Incident Handling Guide)
* **SANS Incident Response Framework**

---

##  Incident Scenario Summary:
* **Attack Type:** Simulated Ransomware / Unauthorized Access
* **Target System:** Virtual Internal Server & User Workstations
* **Severity Level:** High
* **Impact:** Encrypted operational files and suspicious outbound network traffic detected.

---

##  Incident Response Steps (Theory & Execution):

### 1. Preparation & Detection:
* Identified suspicious activities using System Logs and Network Sniffers (Wireshark/SIEM).
* **Indicators of Compromise (IOCs) Identified:**
  * Unrecognized IP communication on non-standard ports.
  * Rapid file encryption and extension changes.
  * Excessive failed login attempts on server accounts.

### 2. Containment Strategy:
* **Immediate Isolation:** Disconnected affected virtual machines from the main network to prevent lateral movement.
* **Account Lockdown:** Temporarily disabled compromised user credentials.
* **Network Segmentation:** Enforced strict firewall rules on remaining active nodes.

### 3. Eradication & Remediation:
* Terminated malicious processes identified in task manager/system processes.
* Conducted full system malware scans using updated security tools.
* Patched identified system vulnerabilities and reset all administrative passwords.

### 4. Recovery & Restoration:
* Restored affected system files from clean, offline backups.
* Monitored network traffic closely for 24–48 hours to confirm system stability.
* Reconnected isolated hosts back to the production environment.

---

## 💡 Post-Incident Analysis & Lessons Learned:
* **Gaps Identified:** Outdated security patches on internal servers and weak password policies.
* **Recommendations:**
  * Implement Multi-Factor Authentication (MFA) across all endpoints.
  * Conduct regular offline backups and vulnerability assessments.
  * Train staff on Phishing awareness and Incident Response drills.

---

##  Repository Structure:
```text
├── docs/
│   └── Incident_Response_Plan_and_Post_Incident_Analysis.docx
├── logs/
│   └── sample_incident_logs.txt
└── README.md
