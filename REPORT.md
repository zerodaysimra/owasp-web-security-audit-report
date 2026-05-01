# Web Application Security Assessment Report

## 📌 Project Overview
This report documents a basic security assessment performed on a vulnerable web application in a controlled lab environment. The objective was to identify common OWASP Top 10 vulnerabilities and understand their impact.

---

## 🎯 Scope
- Target Application: OWASP Juice Shop  
- Environment: Localhost (Lab Setup)  
- Testing Type: Manual Security Testing  

---

## 🛠️ Tools Used
- Burp Suite (Request interception & analysis)  
- Nmap (Network reconnaissance)  
- Web Browser (Manual testing)  

---

## 🔍 Findings Summary

### 1. Cross-Site Scripting (XSS)
- **Risk Level:** Medium  
- **Description:** User input was not properly sanitized, allowing script execution in browser.  
- **Impact:** Client-side script execution  
- **Status:** Confirmed  

---

### 2. SQL Injection (Login Bypass)
- **Risk Level:** High  
- **Description:** Authentication system was vulnerable to SQL injection payloads allowing login bypass.  
- **Impact:** Unauthorized access to application  
- **Status:** Confirmed  

---

### 3. Weak Authentication
- **Risk Level:** High  
- **Description:** Login system allowed authentication using weak or predictable credentials.  
- **Impact:** Unauthorized account access  
- **Status:** Confirmed  

---

## 🌐 Network Reconnaissance
- Port 3000 identified as open using Nmap  
- HTTP service detected running locally  

---

## 📊 Conclusion
The application contains multiple OWASP Top 10 vulnerabilities including XSS, SQL Injection, and Weak Authentication. These issues demonstrate improper input validation and insufficient authentication mechanisms.

---

## ⚖️ Ethical Note
This assessment was conducted in a controlled lab environment for educational purposes only. No real-world systems were targeted.
