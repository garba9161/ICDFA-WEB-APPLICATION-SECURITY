 Web Application Security & Penetration Testing Portfolio  
**Institution:** International Cybersecurity and Digital Forensics Academy (ICDFA)  

---

## Repository Overview

This repository holds my complete academic coursework, technical lab reports, code audits, and penetration testing deliverables completed during **Stage 1** of the Web Application Security and Penetration Testing track at ICDFA. 

The curriculum spans eight modules covering Linux administration, web architecture, vulnerability exploitation, secure coding, input validation, grey-box penetration testing, and enterprise compliance reporting.

---

## Coursework & Deliverables

### Course 1: Foundations of Linux, Networking, and Bash Scripting (`BVWS101`)
Hands-on Linux system administration, network protocol analysis, OSI security mapping, and shell scripting automation.

* 📄 **Linux System Administration Adventure (Users & Packages):** [View Report](./Course-01-Foundations/assignments/Garba%20Work%20Two.pdf)
  * *Overview:* User/group administration (`adduser`, `usermod`, `groupadd`), permission structures (`chmod 755`, `chown`, `chgrp`), and system package management via `apt`.
* 📄 **Networking Fundamentals & IP Addressing:** [View Report](./Course-01-Foundations/assignments/Garba%20Work%20Three.pdf)
  * *Overview:* Flat vs. hierarchical addressing, IANA/RIR delegation, static/dynamic DHCP setups, Classful vs. Classless (CIDR) subnetting, and connectivity troubleshooting.
* 📄 **Research & Analysis — The Attack of the Layers:** [View Report](./Course-01-Foundations/assignments/Garba%20Work%20Four.pdf)
  * *Overview:* OSI 7-layer security assessment mapping layer-specific threats (Phishing at Layer 7, TCP SYN Floods at Layer 4, ARP Spoofing at Layer 2) to mitigation controls (WAF, DAI, SYN Cookies).
* 📄 **Automation with Bash Scripting (20 Exercises):** [View Report](./Course-01-Foundations/assignments/Garba%20Work%20Five.pdf)
  * *Overview:* Scripted automation covering system monitoring (`free -h`, `du -sh`), process management, network diagnostics (`ping`), and automated directory backups.

---

### Course 2: Web Application Security Essentials (`BVWS102`)
A 4-part module on three-tier web architectures, backend development, OWASP risk mapping, and server hardening.

* 📄 **Web Architecture & XSS Vulnerability Identification:** [View Report](./Course-02-Web-Security-Essentials/assignments/Garba%20Assignment%201.pdf)
  * *Overview:* Analysis of client-server-database architecture, event-driven Reflected XSS testing (`onerror`, `onload`, `onclick`), HTML entity escaping (`htmlspecialchars`), and `innerHTML` vs. `textContent` DOM security.
* 📄 **PHP Backend Development with MySQL Database:** [View Report](./Course-02-Web-Security-Essentials/assignments/Garba%20Week%20Two.pdf)
  * *Overview:* XAMPP setup on Kali Linux (`icdfa_lab` database), side-by-side execution of vulnerable vs. secure PHP scripts (SQLi, XSS), and defensive refactoring with Prepared Statements, Bcrypt password hashing, and session regeneration.
* 📄 **OWASP Top 10 Risk Assessment (PayX Secure):** [View Report](./Course-02-Web-Security-Essentials/assignments/Garba%20Week%20Three.pdf)
  * *Overview:* Threat modeling for "PayX Secure" across OWASP risk categories, combined with hands-on exploit validation on OWASP Juice Shop (SQLi auth bypass, DOM XSS, IDOR cart tampering).
* 📄 **Risk Assessment & Secure Application Design:** [View Report](./Course-02-Web-Security-Essentials/assignments/Garba%20Week%20Four.pdf)
  * *Overview:* Encryption analysis (Symmetric, Asymmetric, Hashing), SSL/TLS HTTPS virtual host configuration in XAMPP (`httpd-ssl.conf`), web server hardening (`Options -Indexes`, MySQL root password enforcement), and secure PHP authentication design.

---

### Course 3: OWASP Top 10 Vulnerabilities & Exploitation Techniques (`BVWS103`)
Ten practical lab assignments focused on exploiting and mitigating the OWASP Top 10 vulnerabilities.

* 📄 **Linux Commands & XAMPP Environment Setup:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_0.pdf)
  * *Overview:* Local lab installation using Kali Linux and XAMPP in `/opt/lampp`, permission configuration (`chmod +x`), and initial PHP runtime verification.
* 📄 **SQLi & Command Injection Exploitation (DVWA):** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_Week1.pdf)
  * *Overview:* Manual and automated testing via DVWA. Executed Union-based SQLi, Blind SQLi, OS Command Injection with evasion payloads (`$IFS`, Base64), and SQLMap automated database extraction.
* 📄 **Advanced SQL Injection Exploitation & Mitigation:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_1.pdf)
  * *Overview:* Custom PHP/MySQL app audit, metadata extraction, arbitrary file retrieval (`LOAD_FILE`), Remote Code Execution via web shells (`INTO OUTFILE`), and PDO Prepared Statement remediation.
* 📄 **HTML Injection Exploitation & Mitigation:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_2.pdf)
  * *Overview:* Unvalidated input reflection analysis, inline JavaScript payload execution, and output encoding enforcement via `htmlspecialchars()`.
* 📄 **OS Command Injection Exploitation & Remediation:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_3.pdf)
  * *Overview:* Command chaining exploitation using shell operators (`;`) on a PHP IP ping tool, sanitized using `escapeshellcmd()`.
* 📄 **Cross-Site Scripting (XSS) Exploitation & Remediation:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_4.pdf)
  * *Overview:* Reflected XSS exploitation, cookie theft risk analysis, session hijacking mechanics, and context-aware output encoding.
* 📄 **Broken Access Control Assessment:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_5.pdf)
  * *Overview:* Horizontal and vertical privilege escalation via forced browsing to administrative endpoints, remediated using server-side Role-Based Access Control (RBAC).
* 📄 **Insecure Deserialization Exploitation & Mitigation:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_6.pdf)
  * *Overview:* Exploiting PHP `unserialize()` to manipulate object properties, refactored to safe JSON parsing via `json_decode()`.
* 📄 **Security Misconfiguration & Server Hardening:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_7.pdf)
  * *Overview:* Audit of web server directory listing disclosures and sensitive file exposure (`config.php`). Hardened using web root restructuring and `.htaccess` rules.
* 📄 **Broken Authentication & Session Security:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_8.pdf)
  * *Overview:* Analysis of plaintext credential risks and missing session states. Implemented Bcrypt password hashing (`password_hash()`) and session ID regeneration (`session_regenerate_id()`).

---

### Course 4: Secure Authentication & Access Control (`BVWS104`)
Identity verification systems, access management standards, and authorization enforcement.

* 📄 **Project:** [View Report](./Course-04-Authentication-Access-Control/assignments/Course4_Assignment.pdf)
  * *Overview:* Analysis of authentication protocols (OAuth 2.0, OpenID Connect), Multi-Factor Authentication (MFA) mechanics, session management lifecycles, and RBAC vs. ABAC models.

---

### Course 5: Web Application Penetration Testing Methodologies (`BVWS105`)
Full-scope grey-box ethical hacking engagement targeting the OWASP Juice Shop platform.

* 📄 **OWASP Juice Shop Penetration Testing Report:** [View Report](./Course-05-Penetration-Testing-Methodologies/assignments/GARBA%201.pdf)
  * *Overview:* Application attack surface mapping, SQLi authentication bypass (`' OR 1=1 --`), Reflected XSS, administrative privilege escalation (`/#/administration`), directory traversal on `/ftp` (`coupons_2013.md.bak`), and basket parameter tampering. Delivered with an Executive Summary and Technical Remediation Guide.

---

### Course 6: Secure Coding Practices and Input Validation (`BVWS106`)
Defensive engineering principles, line-by-line vulnerability auditing, and code refactoring.

* 📄 **Secure Coding & Input Validation Assessment:** [View Report](./Course-06-Secure-Coding-Input-Validation/assignments/Assignment%201.pdf)
  * *Overview:* CWE mitigation matrix covering 10 software weaknesses (CWE-89, CWE-521, CWE-307, CWE-598, CWE-613, CWE-384, CWE-79, CWE-352, CWE-285, CWE-209). Includes code audits and fixes for unverified password resets (CWE-640) and IDOR profile access (CWE-639).

---

### Course 7: Compliance, Reporting, and Remediation Strategies (`BVWS107`)
Enterprise incident response, regulatory compliance frameworks, and post-breach remediation.

* 📄 **Compliance, Reporting & Remediation Strategy Report:** [View Report](./Course-07-Compliance-Reporting-Remediation/assignments/Garba%20Assignment%20Report%201.pdf)
  * *Overview:* Case study response to the SecureServe supply chain incident (CVE-2025-12345 SQLi flaw exposing 250,000 metadata records). Evaluated GDPR 72-hour notification mandates for 75,000 EU residents, PCI DSS patching SLAs, Board Executive Briefings, and DevSecOps remediation metrics (MTTR, Flaw Reoccurrence Rate).

---

### Course 8: Stage 1 Capstone Project (`BVWS108`)
Synthesizing offensive testing, defensive engineering, and compliance reporting into an end-to-end audit.

* 📄 **Capstone Final Report:** [View Report](./Course-08-Capstone-Project/assignments/Garba_Capstone_Project.docx)
  * *Overview:* Comprehensive security audit combining black-box vulnerability discovery, manual exploitation, code refactoring, and enterprise compliance reporting.

---

## Directory Structure

```text
.
├── Course-01-Foundations/
│   └── Projects/
├── Course-02-Web-Security-Essentials/
│   └── Projects/
├── Course-03-OWASP-Top-10-Exploitation/
│   └── Projects/
├── Course-04-Authentication-Access-Control/
│   └── Projects/
├── Course-05-Penetration-Testing-Methodologies/
│   └── Projects/
├── Course-06-Secure-Coding-Input-Validation/
│   └── Projects/
├── Course-07-Compliance-Reporting-Remediation/
│   └── Projects/
├── Course-08-Capstone-Project/
│   └── Projects/
└── README.md

```

---

## Licensing & Usage

These lab deliverables were created as part of the **International Cybersecurity and Digital Forensics Academy (ICDFA)** Web Application Security Programme and are shared strictly for educational and portfolio demonstration purposes.

---

## Contact

* **LinkedIn:** [Garba](https://www.limkedin.com/in/ahmed-garba-40b501250?)
* **GitHub:** [@garba9161](https://github.com/garba9161)
```

```
