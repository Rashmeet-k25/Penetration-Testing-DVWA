# Finding Log

---

## Finding ID

F-001

---

## Finding Title

SQL Injection (CWE-89)

---

## Severity

High

---

## Status

Confirmed

---

## Target Application

DVWA (Damn Vulnerable Web Application)

---

## Affected Module

SQL Injection

---

## Affected Parameter

id

---

## HTTP Method

GET

---

## Vulnerability Classification

- OWASP Top 10 2021: A03 - Injection
- CWE-89: Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection')

---

## Description

During the security assessment of the DVWA SQL Injection module, the application was found to process user-controlled input through the "id" parameter without adequate input validation or parameterized database queries.

Testing confirmed that crafted input influenced backend SQL query execution. The application disclosed verbose MariaDB error messages when malformed input was processed, revealing internal implementation details including database type, PHP function names, file paths, and source code line numbers.

Further testing demonstrated that the vulnerability allowed retrieval of backend database information including:

- Database version
- Current database name
- Database schema
- Table names
- Column names
- User-related information

These findings confirm the presence of a SQL Injection vulnerability.

---

## Evidence

**E-008** – SQL Injection Module

**E-009** – Baseline Application Response

**E-010** – SQL Syntax Error Disclosure

**E-011** – Successful SQL Injection Validation

**E-012** – Database Version Disclosure

**E-013** – Database Enumeration

**E-014** – Table and Column Enumeration

**E-015** – User Information Disclosure

---

## Security Impact

The vulnerability allows an attacker to manipulate SQL queries executed by the application.

Potential consequences include:

- Disclosure of sensitive database information
- Enumeration of database structure
- Exposure of application data
- Increased attack surface through verbose error messages
- Potential privilege escalation depending on deployment configuration

---

## Business Impact

Successful exploitation could expose confidential organizational or customer information, resulting in loss of confidentiality, regulatory non-compliance, reputational damage, and financial loss.

---

## Risk Rating

High

---

## Recommended Remediation

- Use prepared statements with parameterized queries.
- Perform strict server-side input validation.
- Disable verbose SQL error messages in production.
- Apply the principle of least privilege to database accounts.
- Conduct secure code reviews and regular penetration testing.

---

## Finding Status

Confirmed
