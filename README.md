# DVWA Web Application Penetration Test

## Overview

This repository contains a complete web application penetration testing project performed against the **Damn Vulnerable Web Application (DVWA)** in a controlled laboratory environment. The project follows a structured penetration testing methodology to identify, validate, assess, and document a **SQL Injection** vulnerability, along with its technical and business impact.

The objective of this project is to demonstrate practical web application security testing skills, professional documentation, and reporting practices commonly used in real-world penetration testing engagements.

---

## Objectives

- Set up and configure a secure penetration testing lab.
- Perform web application security testing against DVWA.
- Identify and validate a SQL Injection vulnerability.
- Capture and document supporting evidence.
- Assess technical and business impact.
- Provide risk analysis and remediation recommendations.
- Produce a professional penetration testing report.

---

## Scope

**Target Application:** Damn Vulnerable Web Application (DVWA)

**Assessment Type:** Web Application Penetration Test

**Environment:** Local Kali Linux Lab

**Framework:** OWASP Web Security Testing Guide (WSTG)

---

## Repository Structure

```text
DVWA-Pentest-Project/
│
├── Diagrams/          # Kill Chain and supporting diagrams
├── Evidence/          # Evidence logs and finding documentation
├── Notes/             # Assessment notes, risk analysis, and remediation
├── Reports/           # Final penetration testing report
├── Screenshots/       # Screenshots collected during testing
└── README.md
```

---

## Methodology

The assessment followed a structured penetration testing workflow:

1. Planning & Scope Definition
2. Lab Setup
3. Reconnaissance
4. HTTP Traffic Analysis
5. SQL Injection Testing
6. Vulnerability Validation
7. Evidence Collection
8. Risk Assessment
9. Remediation Planning
10. Report Writing

---

## Tools Used

- Kali Linux
- DVWA
- Burp Suite Community Edition
- Firefox
- Apache
- MariaDB

---

## Key Finding

| Finding | Severity | Status |
|---------|----------|--------|
| SQL Injection (CWE-89) | High | Confirmed |

The assessment confirmed a **High Severity SQL Injection** vulnerability affecting the `id` parameter of the DVWA SQL Injection module. Successful testing demonstrated unauthorized disclosure of backend database information, including database details, schema information, and user-related records.

---

## Skills Demonstrated

- Web Application Penetration Testing
- SQL Injection Testing
- HTTP Request Analysis
- Burp Suite Traffic Interception
- Vulnerability Validation
- Risk Assessment
- Technical Documentation
- Penetration Testing Reporting
- OWASP WSTG Methodology

---

## Disclaimer

This project was conducted **exclusively within an authorized local laboratory environment** using the Damn Vulnerable Web Application (DVWA). It is intended for educational purposes and cybersecurity skill development only. No unauthorized systems or networks were tested.

---

## Author

**Rashmeet Kaur**

Cybersecurity | Web Application Security | VAPT | Penetration Testing

This repository is part of my cybersecurity portfolio showcasing hands-on penetration testing projects and professional security documentation.
