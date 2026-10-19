# Endpoint Protection Lab – Trend Micro Deep Security

**Hands-on Lab: Deploying Trend Micro Deep Security Agent & Detecting Malware**

This repository documents a practical cybersecurity lab where I deployed the Trend Micro Deep Security agent on a Windows VM, enabled Anti-Malware protection, detected and quarantined the EICAR test file, reviewed alerts, and documented the findings in an incident report.

---

##  Tools Used

| Tool                          | Purpose                              |
|-------------------------------|--------------------------------------|
| Trend Micro Deep Security     | Endpoint Protection Platform (EPP)   |
| Deep Security Agent           | Endpoint agent installed on VM       |
| Windows 10/11 VM              | Target endpoint                      |
| EICAR Test File               | Safe malware simulation file         |
| Deep Security Manager (DSM)   | Central management console           |

---

##  Lab Objectives

1. Deploy Trend Micro Deep Security Agent on a Windows lab VM
2. Enable Anti-Malware protection module
3. Download and execute the EICAR test file
4. Verify detection, quarantine, and alert generation
5. Review and classify the security event
6. Document findings in a formal incident report

---

##  Lab Setup

- **Endpoint**: Windows 10/11 Virtual Machine
- **Protection**: Trend Micro Deep Security Agent with Anti-Malware module enabled
- **Test File**: EICAR Standard Anti-Virus Test File (`eicar.com`)
- **Management**: Deep Security Manager console for policy and alert review

---

##  Steps Performed

### 1. Agent Deployment
- Installed Deep Security Agent on the Windows VM
- Activated the agent with Deep Security Manager
- Assigned a security policy with **Anti-Malware** enabled

### 2. Anti-Malware Configuration
- Enabled Real-time Scan
- Enabled Scheduled Scan
- Set action for malware: **Quarantine / Clean**
- Enabled alert generation for detections

### 3. Malware Simulation
- Downloaded the official EICAR test file
- Attempted to execute / open the file
- Deep Security immediately detected and quarantined it

### 4. Alert Review & Classification
- Reviewed the generated alert in Deep Security Manager
- Classified the event as **True Positive – Test Malware**
- Noted detection name, action taken, and file path

---

##  Key Findings

- Deep Security Agent successfully detected the EICAR test file in real-time
- File was automatically quarantined
- Alert was generated with clear details (malware name, severity, action)
- Event classification: **True Positive** (intentional test)
- No false positives observed during the lab

---

##  Recommendations

1. Keep Anti-Malware patterns and engine up to date
2. Enable Behavior Monitoring and Predictive Machine Learning if available
3. Configure email / SIEM forwarding for critical malware alerts
4. Regularly test detection using EICAR or other safe test files
5. Document all test activities to avoid confusion with real incidents

---

##  Repository Structure

```
Endpoint-Protection-Lab-Trend-Micro/
├── README.md
├── configs/
│   └── anti-malware-policy-notes.md
├── logs/
│   └── detection-alert-sample.txt
├── docs/
│   └── incident-report.md
└── screenshots/
    └── README.md
```

---

##  Author

**Manoj Kumar V M**  
Cybersecurity Enthusiast | SOC Analyst Aspirant  

- GitHub: [github.com/manojkumarvm](https://github.com/manojkumarvm)
- Email: manumanoj2422@gmail.com

---

**Note**: This is a personal learning lab. The EICAR file is a harmless test file designed specifically for antivirus testing and contains no actual malicious code.
