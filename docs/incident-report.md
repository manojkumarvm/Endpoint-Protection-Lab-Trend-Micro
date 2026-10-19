# Incident Report – Endpoint Protection Lab

**Report ID**: LAB-DS-001  
**Date**: 19 October 2026  
**Prepared by**: Manoj Kumar V M  
**Classification**: Lab / Training Exercise  

---

## 1. Summary

A controlled malware detection test was performed using the EICAR standard test file on a Windows virtual machine protected by Trend Micro Deep Security. The Deep Security Agent successfully detected, quarantined, and generated an alert for the test file.

---

## 2. Environment Details

| Item                    | Details                          |
|-------------------------|----------------------------------|
| Endpoint                | Windows 10/11 VM                 |
| Protection Solution     | Trend Micro Deep Security        |
| Module Enabled          | Anti-Malware                     |
| Test File               | EICAR Standard Anti-Virus Test File |
| Detection Method        | Real-time Scan                   |

---

## 3. Timeline of Events

| Time       | Event                                      |
|------------|--------------------------------------------|
| 10:10      | Deep Security Agent installed & activated  |
| 10:12      | Anti-Malware policy applied                |
| 10:14      | EICAR test file downloaded                 |
| 10:15      | File detected and quarantined              |
| 10:16      | Alert reviewed in Deep Security Manager    |
| 10:20      | Findings documented                        |

---

## 4. Detection Details

- **Malware Name**: EICAR-Test-File
- **Action Taken**: Quarantined
- **File Path**: C:\Users\LabUser\Downloads\eicar.com
- **Severity**: High
- **Scan Type**: Real-time

---

## 5. Classification

**True Positive** – The detection was expected and intentional as part of the lab exercise. No real threat was present.

---

## 6. Actions Taken

1. Confirmed the file was quarantined
2. Reviewed the full alert details
3. Documented the event for learning purposes
4. No remediation required beyond quarantine (test file)

---

## 7. Lessons Learned

- Trend Micro Deep Security Anti-Malware module responds quickly to known test signatures
- Real-time protection is effective for immediate detection
- Proper documentation of test activities is important to avoid confusion with real incidents

---

## 8. Recommendations

- Maintain up-to-date malware patterns
- Regularly validate detection capability using safe test files (EICAR)
- Configure alert forwarding to SIEM or email for operational visibility
- Include similar tests in regular health-check procedures

---

**End of Report**
