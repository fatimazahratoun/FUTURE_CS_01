# 🔐 Web Application Penetration Testing - DVWA

**Author:** Fatima Zahrae Khalil  
**Project:** Future Interns - Cybersecurity Task 1  
**Date:** December 2025

## 📁 Project Structure
Cybersecurity-Pentest-DVWA/
│
├── 📄 README.md # This file
├── 📄 SECURITY_TESTING_REPORT.pdf # Complete penetration testing report
│
├── 📂 src/ # Exploitation payloads
│ ├── 📂 sql-injection/
│ │ └── payloads.txt # SQL injection test payloads
│ ├── 📂 xss/
│ │ └── payloads.txt # XSS test payloads
│ └── 📂 csrf/
│ └── payloads.txt # CSRF test payloads
│
├── 📂 logs/ # Burp Suite traffic logs
│ ├── burp_history_SQL.xml # SQL injection traffic
│ ├── burp_history_XSS.xml # XSS testing traffic
│ └── burp_history_CSRF.xml # CSRF testing traffic
│
└── 📂 documentation/ # Additional documentation
├── METHODOLOGY.md # Testing methodology
├── TOOLS_SETUP.md # Environment setup guide
├── TESTING_PROCEDURE.md # Step-by-step testing procedures
└── BURP_LOGS_GUIDE.md # How to analyze Burp logs

## 🔍 Overview

This repository contains the complete documentation, payloads, and evidence from a comprehensive penetration test conducted on the Damn Vulnerable Web Application (DVWA). The assessment focused on identifying and exploiting critical web application vulnerabilities including SQL Injection, Cross-Site Scripting (XSS), and Cross-Site Request Forgery (CSRF).

## 🎯 Key Components

### 1. **Security Report** (`SECURITY_TESTING_REPORT.pdf`)
Complete professional penetration testing report with:
- Executive summary and risk assessment
- Detailed vulnerability findings
- Proof of concept evidence
- Remediation recommendations
- Business impact analysis

### 2. **Exploitation Payloads** (`src/`)
Organized collection of test payloads:
- **SQL Injection:** 50+ boolean, union, error-based, and blind SQLi payloads
- **XSS:** 40+ reflected, stored, and DOM-based XSS payloads
- **CSRF:** Various CSRF attack vectors and bypass techniques

### 3. **Traffic Logs** (`logs/`)
Burp Suite HTTP traffic captures:
- `burp_history_SQL.xml`: SQL injection attack sequences
- `burp_history_XSS.xml`: XSS exploitation traffic
- `burp_history_CSRF.xml`: CSRF attack demonstrations

## 🛠️ Usage Instructions

### Viewing the Report
Open `SECURITY_TESTING_REPORT.pdf` with any PDF reader.

### Analyzing Traffic Logs
```bash
# Import into Burp Suite
1. Open Burp Suite Professional/Community
2. Go to Proxy → HTTP History
3. Import the XML files from logs/ directory
4. Analyze request/response sequences
## ⚙️ Prerequisites

- [DVWA](http://www.dvwa.co.uk/) installed and configured
- [Burp Suite](https://portswigger.net/burp) (Community or Professional)
- Local web server (XAMPP, WAMP, Docker, etc.)
- Browser with proxy configured (e.g., 127.0.0.1:8080)
## 🚨 Identified Vulnerabilities

| Vulnerability | Risk Level | Status |
|---------------|------------|--------|
| SQL Injection (Union-based) | High | Exploited |
| Stored XSS | Medium | Exploited |
| CSRF | Medium | Exploited |
[📋 View Full Report](SECURITY_TESTING_REPORT.pdf)