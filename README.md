# Web Application Security & Penetration Testing Projects

This repository covers lab projects, code reviews, and penetration testing reports I have submitted as part of the International Cybersecurity and Digital Forensics Academy (ICDFA) Web Application Security Programme.

---

## BVWS101: Foundations of Cybersecurity & Web Technologies

An introduction to fundamental web protocols, client-server communication models, and web application threat landscapes.

* 📄 **Course Assignment:** [View Report](./Course-01-Foundations/assignments/Course1_Assignment.pdf)
  * *Briefing:* Overview of HTTP/HTTPS request-response lifecycles, TCP/IP mechanics, browser security boundaries, cookie/session state management, and baseline threat modeling.

---

## BVWS102: Web Application Security Essentials

Covers essential components of web application architecture, data handling, and common web vulnerabilities.

* 📄 **Course Assignment:** [View Report](./Course-02-Web-Security-Essentials/assignments/Course2_Assignment.pdf)
  * *Briefing:* Analysis of three-tier web architectures, client-side vs. server-side input validation, PHP and MySQL backend interactions, session cookie security attributes, and introductory Cross-Site Scripting (XSS).

---

## BVWS103: OWASP Top 10 Vulnerabilities & Exploitation Techniques

A comprehensive series of 10 practical lab assignments focused on identifying, exploiting, and remediating the OWASP Top 10 vulnerabilities.

* 📄 **Lab 0 — Linux Commands & XAMPP Environment Setup:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_0.pdf)
  * *Briefing:* Local web security lab installation using Kali Linux and XAMPP in `/opt/lampp`, directory permissions management (`chmod +x`), repository updates, and initial PHP environment testing[cite: 19].

* 📄 **Week 1 Lab — SQLi & Command Injection Exploitation (DVWA):** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_Week1.pdf)
  * *Briefing:* Manual and automated exploitation using Damn Vulnerable Web Application (DVWA). Covers Union-based SQLi, Boolean/Time-based Blind SQLi, OS Command Injection with shell evasion (`$IFS`, Base64), out-of-band data exfiltration, and SQLMap database dumping (`--dbs`, `--dump`, `--os-shell`)[cite: 18].

* 📄 **Lab 1 — Advanced SQL Injection Exploitation & Mitigation:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_1.pdf)
  * *Briefing:* Custom PHP/MySQL vulnerable web app development, system metadata extraction, database dumping, arbitrary file retrieval (`LOAD_FILE`), Remote Code Execution via web shells (`INTO OUTFILE`), and fixing via PDO Prepared Statements[cite: 20].

* 📄 **Lab 2 — HTML Injection Exploitation & Mitigation:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_2.pdf)
  * *Briefing:* Building reflected input forms, executing inline JavaScript alert payloads, analyzing unvalidated input reflection in the DOM, and applying output encoding via `htmlspecialchars()`[cite: 21].

* 📄 **Lab 3 — OS Command Injection Exploitation & Remediation:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_3.pdf)
  * *Briefing:* Developing an IP ping utility in PHP, exploiting command chaining using shell operators (`;`), and implementing command sanitization using `escapeshellcmd()`[cite: 22].

* 📄 **Lab 4 — Cross-Site Scripting (XSS) Exploitation & Remediation:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_4.pdf)
  * *Briefing:* Practical exploitation of Reflected XSS flaws, session hijacking risk analysis, cookie theft mechanisms, and applying strict context-aware output encoding[cite: 23].

* 📄 **Lab 5 — Broken Access Control Assessment:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_5.pdf)
  * *Briefing:* Simulating horizontal and vertical privilege escalation via forced browsing to unlinked administrative endpoints, implementing server-side Role-Based Access Control (RBAC), and enforcing a "Deny by Default" model[cite: 24].

* 📄 **Lab 6 — Insecure Deserialization Exploitation & Mitigation:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_6.pdf)
  * *Briefing:* Exploiting PHP `unserialize()` to manipulate object properties for privilege escalation, and refactoring backend code to safely parse data using `json_decode()`[cite: 25].

* 📄 **Lab 7 — Security Misconfiguration & Server Hardening:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_7.pdf)
  * *Briefing:* Audit of web server misconfigurations including exposed directory listings and sensitive file leakage (`config.php`, `.htaccess`). Implemented web root file migration and `.htaccess` access restrictions[cite: 26].

* 📄 **Lab 8 — Broken Authentication & Session Security:** [View Report](./Course-03-OWASP-Top-10-Exploitation/assignments/Garba_8.pdf)
  * *Briefing:* Assessing risks of plaintext credential storage and missing session states. Upgraded login mechanisms to Bcrypt hashing (`password_hash()`, `password_verify()`) and implemented secure session renewal (`session_regenerate_id(true)`)[cite: 27].

---

## BVWS104: Secure Authentication & Access Control

Explores identity verification, access management standards, and authorization enforcement.

* 📄 **Course Assignment:** [View Report](./Course-04-Authentication-Access-Control/assignments/Course4_Assignment.pdf)
  * *Briefing:* In-depth analysis of authentication protocols (OAuth 2.0, OpenID Connect), Multi-Factor Authentication (MFA) implementation, session management lifecycles, and access control models (RBAC vs. ABAC).

---

## BVWS105: Web Application Penetration Testing Methodologies

A full-scope ethical hacking assessment executed against the target application (OWASP Juice Shop).

* 📄 **OWASP Juice Shop Penetration Testing Report:** [View Report](./Course-05-Penetration-Testing-Methodologies/assignments/GARBA_1.pdf)
  * *Briefing:* Complete penetration testing engagement covering:
    * **Recon Mapping:** Documenting entry points across search, login, registration, contact, user profile, cart, and FTP directory endpoints[cite: 28, 29].
    * **Exploitation:** Executing SQLi login bypass (`' OR 1=1 --`), DOM Reflected XSS, privilege escalation to `/administration`, directory traversal under `/ftp` (`coupons_2013.md.bak`), and basket parameter tampering[cite: 28, 29].
    * **Reporting:** Executive Summary for leadership alongside a Technical Vulnerability Deep-Dive with remediation recommendations (Prepared Statements, CSP, server-side RBAC)[cite: 29].

---

## BVWS106: Secure Coding Practices and Input Validation

Defensive engineering principles, line-by-line vulnerability auditing, and code refactoring.

* 📄 **Secure Coding & Input Validation Assessment:** [View Report](./Course-06-Secure-Coding-Input-Validation/assignments/Assignment_1.pdf)
  * *Briefing:* Structured into three core analysis areas:
    * **CWE Matrix:** Remediation strategies for CWE-89 (SQLi), CWE-521 (Weak Passwords), CWE-307 (Brute Force), CWE-598 (GET Exposure), CWE-613 (Session Expiration), CWE-384 (Session Fixation), CWE-79 (XSS), CWE-352 (CSRF), CWE-285 (Access Control), and CWE-209 (Error Leaks)[cite: 29].
    * **Authentication & Authorization Audits:** Analyzing GET parameter credential exposure, weak MD5 hashing, unverified password resets (CWE-640), IDOR profile access (CWE-639), and URL role tampering[cite: 29].
    * **Defensive Code Fixes:** Refactoring vulnerable PHP and Python code bases to enforce Parameterized Queries, secure session roles, and context-aware output encoding (`htmlspecialchars()`)[cite: 29].

---

## BVWS107: Compliance, Reporting, and Remediation Strategies

Enterprise incident response, regulatory compliance frameworks, and post-breach remediation.

* 📄 **Compliance, Reporting & Remediation Strategy Report:** [View Report](./Course-07-Compliance-Reporting-Remediation/assignments/Garba_Assignment_Report_1.pdf)
  * *Briefing:* Strategic response to the SecureServe supply chain incident involving a third-party library SQLi vulnerability (CVE-2025-12345) exposing 250,000 user metadata records[cite: 30]. Covers GDPR regulatory reporting (72-hour notification for 75,000 affected EU users), PCI DSS patch SLAs, Board-level Executive Summaries, Engineering Technical Briefings, and DevSecOps remediation metrics (MTTR, Flaw Reoccurrence Rate)[cite: 30].

---

## BVWS108: Stage 1 Capstone Project

The final stage assessment synthesizing offensive testing, defensive engineering, and compliance reporting.

* 📄 **Capstone Final Report:** [View Report](./Course-08-Capstone-Project/assignments/Course8_Capstone.pdf)
  * *Briefing:* End-to-end security assessment combining black-box vulnerability discovery, exploit validation, secure code refactoring, and enterprise compliance reporting into a unified final audit.

---

## Contribution & Licensing

These lab deliverables were created as part of the **International Cybersecurity and Digital Forensics Academy (ICDFA)** Web Application Security Programme and are shared strictly for educational and research purposes. Feel free to open an issue or submit a pull request if you find any bugs or have suggested improvements.

---

## Contact & Connect

For inquiries, feedback, or technical discussions, feel free to reach out:

* **LinkedIn:** [Ahmed Garba](https://linkedin.com)
