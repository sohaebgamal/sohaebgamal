<div align="center">

# Sohaib Gamal

**Security QA Engineer & Penetration Tester** &nbsp;·&nbsp; Web, API & Business-Logic Security

Full-cycle offensive engagements — *reconnaissance → exploitation → professional reporting* — mapped to the **OWASP Top 10** and the **Cyber Kill Chain**.

<p>
  <img src="https://img.shields.io/badge/TryHackMe-Top%202%25%20Globally-c11111?style=for-the-badge&logo=tryhackme&logoColor=white" alt="THM Top 2%"/>
  <img src="https://img.shields.io/badge/Rooms-164%2B-1f6feb?style=for-the-badge&logo=hackthebox&logoColor=white" alt="164 Rooms"/>
  <img src="https://img.shields.io/badge/Level-12%20Sapphire-f0a500?style=for-the-badge" alt="Level 12"/>
  <img src="https://img.shields.io/badge/Specialism-Red%20Team-black?style=for-the-badge" alt="Red"/>
</p>

<a href="https://www.linkedin.com/in/sohaeb-gamal-a14205342/">LinkedIn</a> &nbsp;•&nbsp;
<a href="https://tryhackme.com/p/sohaeb">TryHackMe</a> &nbsp;•&nbsp;
<a href="mailto:sebeko.1996@gmail.com">Email</a> &nbsp;•&nbsp;
📍 Alexandria, Egypt

</div>

---

## 🎯 Profile

Security QA Engineer and Penetration Tester covering **web and API products**, owning both functional QA and offensive security testing. Two independently confirmed **CRITICAL account-takeover chains** reported and tracked through remediation and retest, with hands-on experience taking engagements end-to-end: identifying and exploiting high-impact vulnerabilities, chaining them through to host and domain compromise, and delivering bilingual (Arabic/English) client-ready reports with CVSS/CWE mapping, proof-of-concept evidence, and prioritized remediation.

An active builder of **custom Python tooling** that automates discovery and extends manual coverage (Dagger, VulnScan AI, VulnScan-HEX, IDOR Tester).

---

## 💼 Experience

- **Security QA Engineer & Penetration Tester — SmartWare Ltd** *(Jan 2025 – Jan 2026 · Full-time)*
  Functional QA and offensive security testing for an admin/workflow platform, a payments API platform and two ride-hailing platforms (web and API).
  - Full black-box assessments of web and API platforms: **9 findings** on one engagement (broken access control CWE-862, unauthenticated Swagger/OpenAPI exposure of ~190 endpoints CWE-200, IDOR exposing PII CWE-639, user enumeration, missing login rate-limiting), chained into **2 independently confirmed CRITICAL account-takeover paths**.
  - Stored XSS (HIGH) on a public preview domain and CSV formula injection (CWE-1236) via exported spreadsheets.
  - Login rate-limit and brute-force resilience testing that exposed a server capacity collapse (502) and a Redis misconfiguration.
  - Closing all CRITICAL/HIGH findings cut the CVSS-weighted risk score by **~80%** (payments platform) and **~75%** (ride-hailing platform).
  - Owned manual QA across 9 modules: test plans, module-level test cases, regression and retesting.
- **Freelance Security Engineer** *(2024 – 2025)*
  - **VulnScan AI** — co-designed and owned a vulnerability scanner that verifies every finding against the live target before reporting; in one real test, 38 raw results were filtered to 7 confirmed.
  - **AqarMap** — independent OWASP Top 10 web application pentest; reported authentication weaknesses and business-logic flaws with remediation guidance.

✍️ **Writing:** [VulnScan-HEX — a scanner that proves, not guesses](posts/vulnscan-hex-architecture.md)

🟢 Open to **remote contract / part-time** work in penetration testing, application security and security QA.

---

## 🧠 Areas of Expertise

| Domain | Focus |
|---|---|
| **Web Application** | SQL Injection (Union/Blind/Time) · XSS (Reflected/Stored/DOM) · IDOR · CSRF · SSRF · LFI/RFI · Broken Authentication · Security Misconfigurations |
| **Advanced Web Attacks** | JWT Algorithm Confusion (RS256→HS256) & token forgery · HTTP Request Smuggling (CL.TE / TE.CL) · OAuth CSRF · Race Conditions |
| **Active Directory** | Enumeration · Kerberos abuse (AS-REP / S4U2Self / constrained delegation) · Lateral Movement (PtH, WinRM, PsExec) · Credential Harvesting · DCSync → Domain Admin |
| **API & Auth Testing** | REST API assessment · authentication & token-flow analysis · BOLA · Mass Assignment · rate-limiting abuse |
| **Network & Recon** | Nmap (NSE) · Wireshark · ARP/DNS spoofing · HTTPS downgrade · session hijacking · WiFi (WEP/WPA2, Evil Twin) · OSINT |
| **Post-Exploitation** | Privilege escalation (Linux/Windows) · pivoting & tunneling · hash cracking (hashcat/john) |

---

## 🛠️ Tech Stack

<p>
  <img src="https://img.shields.io/badge/Burp%20Suite-FF6633?style=flat-square&logo=burpsuite&logoColor=white"/>
  <img src="https://img.shields.io/badge/Metasploit-2596CD?style=flat-square&logo=metasploit&logoColor=white"/>
  <img src="https://img.shields.io/badge/BloodHound-AD2B2B?style=flat-square"/>
  <img src="https://img.shields.io/badge/Impacket-4B275F?style=flat-square"/>
  <img src="https://img.shields.io/badge/Nmap-4682B4?style=flat-square"/>
  <img src="https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white"/>
  <img src="https://img.shields.io/badge/ffuf-000000?style=flat-square"/>
  <img src="https://img.shields.io/badge/OWASP-000000?style=flat-square&logo=owasp&logoColor=white"/>
</p>
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white"/>
  <img src="https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black"/>
  <img src="https://img.shields.io/badge/Kali%20Linux-557C94?style=flat-square&logo=kalilinux&logoColor=white"/>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black"/>
  <img src="https://img.shields.io/badge/Active%20Directory-0078D4?style=flat-square&logo=windows&logoColor=white"/>
</p>

---

## 📂 Featured Repositories

<table>
  <tr>
    <td width="33%" valign="top">
      <h3>🛡️ <a href="https://github.com/sohaebgamal/pentest-writeups">pentest-writeups</a></h3>
      17 client-style pentest reports — AD domain compromises (Dead Drop, Silent Monitor), host/web exploitation, cloud SSRF→IMDS, LLM pentesting & methodology.<br><br>
      <i>Executive summary → attack chain → remediation.</i>
    </td>
    <td width="33%" valign="top">
      <h3>🧰 <a href="https://github.com/sohaebgamal/pentest-tools">pentest-tools</a></h3>
      Custom Python tooling: <b>Dagger</b> (password-reset auditor), <b>VerboseLogin_UserEnum</b>, <b>IDOR Tester</b>, <b>loc-tracker</b>, and a recon script suite.
    </td>
    <td width="33%" valign="top">
      <h3>📚 <a href="https://github.com/sohaebgamal/pentest-notes">pentest-notes</a></h3>
      Structured Arabic knowledge base — 16 modules on web attacks, SQLi/XSS/CSRF, API security, Active Directory & testing frameworks.
    </td>
  </tr>
</table>

---

## 🚩 Selected Engagements

> Lab engagements (TryHackMe) documented as full client-style reports. Click any name for the report.

| Engagement | Type | Key techniques | Outcome |
|---|---|---|---|
| [**Dead Drop**](https://github.com/sohaebgamal/pentest-writeups/blob/main/active-directory/dead-drop.md) | Web → AD | SQLi auth bypass → Node `require()` RCE → leaked creds → hardcoded domain creds in APK → AD ACL abuse (nested Domain Admins) | 🔴 **Domain Admin** |
| [**Silent Monitor**](https://github.com/sohaebgamal/pentest-writeups/blob/main/active-directory/silent-monitor.md) | Web → Host | SQLi + command injection → SSH foothold → cracked KeePass (KDBX4) vault → privesc | 🔴 **Root** |
| [**Intro to AD Lateral Movement**](https://github.com/sohaebgamal/pentest-writeups/blob/main/active-directory/intro-to-ad-lateral-movement.md) | Active Directory | PsExec / WinRM · Pass-the-Hash · local-admin reuse · SOCKS pivot to DC | 🔴 **Domain Admin** (5/5 flags) |
| [**Jump**](https://github.com/sohaebgamal/pentest-writeups/blob/main/host-and-web/jump.md) | Linux Host | Anonymous FTP recon → PATH hijack → `sudo deploy.sh` → `sudo less` GTFOBin | 🔴 **Root** (5/5 flags) |
| [**Tomcat CVE-2024-50379**](https://github.com/sohaebgamal/pentest-writeups/blob/main/host-and-web/tomcat-cve-2024-50379.md) | Web Server | TOCTOU race-condition RCE on Apache Tomcat 10.1.x → reverse shell | 🔴 **RCE** |
| [**Cloud Security Fundamentals**](https://github.com/sohaebgamal/pentest-writeups/blob/main/emerging-tech/cloud-security-fundamentals.md) | Cloud | SSRF → IMDS credential theft → role assumption → production secrets | 🔴 **Cloud creds** |

📄 Full report library → **[pentest-writeups](https://github.com/sohaebgamal/pentest-writeups)**

---

## 🔬 Custom Tooling Highlights

- **VulnScan-HEX** — modular web vulnerability scanner in Python built on Hexagonal Architecture (Ports & Adapters). The core only judges evidence (request/response), so findings are verified rather than pattern-matched; 15 scanners aligned with OWASP Top 10:2025 (SQLi, XSS, SSRF, SSTI, RCE, JWT, GraphQL), local AI reporting via Ollama, 30 unit tests.
- **Dagger** — authentication and rate-limit testing platform; its password-reset auditor: detects tokens leaked in API responses, scores token entropy to flag brute-forceable values, checks user enumeration & rate-limiting, and emits ready-to-run `crunch`/`ffuf`/`hydra` recipes.
- **VerboseLogin_UserEnum** — discovers valid accounts by diffing login error responses (auto-baseline + marker modes), producing spray-ready output.

---

## 📜 Certifications & Training

- **TryHackMe — Junior Penetration Tester** *(Top 2% globally · 164 rooms · Level 12)*
- **CompTIA Security+** — training completed; exam in preparation
- Additional: Network Penetration Testing (WiFi & Wired) · Social Engineering awareness · Advanced C Programming

---

<div align="center">

<a href="https://www.linkedin.com/in/sohaeb-gamal-a14205342/"><img src="https://img.shields.io/badge/LinkedIn-Sohaib%20Gamal-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
<a href="https://tryhackme.com/p/sohaeb"><img src="https://img.shields.io/badge/TryHackMe-sohaeb-c11111?style=flat-square&logo=tryhackme&logoColor=white"/></a>
<a href="mailto:sebeko.1996@gmail.com"><img src="https://img.shields.io/badge/Email-sebeko.1996@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white"/></a>

<sub><i>Offensive security for defense — authorized testing only.</i></sub>

</div>
