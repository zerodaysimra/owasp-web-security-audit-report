# OWASP Web Security Audit Report

## 📌 Overview
This project demonstrates a structured web application security audit based on OWASP Top 10 principles. The goal is to identify common vulnerabilities, analyze their impact, and suggest remediation strategies.

---

## 🎯 Objectives
- Identify common web application vulnerabilities  
- Understand real-world attack patterns  
- Perform basic vulnerability assessment  
- Document findings in a structured format  

---

## 🛠️ Tools Used
- Burp Suite  
- Nmap  
- Web Browser  

---

## 🔍 Scope of Testing
The assessment was performed on a deliberately vulnerable web application in a controlled lab environment for educational purposes. No real-world systems were targeted.

---

## ⚠️ Vulnerabilities Identified

### 1. Cross-Site Scripting (XSS)
- **Risk Level:** Medium  
- **Description:** User input was not properly validated  
- **Impact:** Malicious scripts can run in the user’s browser  
- **Fix:** Input validation and output encoding  

---

### 2. SQL Injection (Basic)
- **Risk Level:** High  
- **Description:** Application did not sanitize user input in queries  
- **Impact:** Unauthorized database access  
- **Fix:** Use parameterized queries  

---

### 3. Weak Authentication
- **Risk Level:** Medium  
- **Description:** Weak/default credentials allowed access  
- **Impact:** Unauthorized login  
- **Fix:** Enforce strong password policies  

---

## 📊 Key Learnings
- Practical understanding of OWASP Top 10  
- Importance of secure input handling  
- Basics of vulnerability identification and reporting  

---

## ⚖️ Ethical Note
This project was conducted in a controlled lab environment for educational purposes only.
