# OWASP Web Security Audit Report

## 📌 Overview
This project demonstrates a practical web application security assessment based on OWASP Top 10 principles. The objective was to identify, analyze, and document common web vulnerabilities in a controlled lab environment using industry-relevant tools and methodologies.

---

## 🎯 Objectives
- Perform vulnerability assessment on a web application  
- Identify and analyze common security flaws  
- Demonstrate real-world exploitation scenarios  
- Document findings in a structured VAPT-style report  

---

## 🛠️ Tools Used
- Burp Suite (intercepting proxy & request analysis)  
- Nmap (basic reconnaissance)  
- Web Browser (manual testing)  

---

## 🔍 Scope of Testing
Testing was conducted on a deliberately vulnerable application in a controlled lab environment. No real-world systems or user data were targeted.

---

## ⚠️ Vulnerabilities Identified

---

### 1. Cross-Site Scripting (XSS)

- **Risk Level:** Medium  
- **Type:** Stored / DOM-based XSS  
- **Description:** User input was not properly sanitized before being processed and rendered, allowing injection of malicious JavaScript.  
- **Impact:** Attackers can execute scripts in the victim’s browser, potentially leading to session hijacking or data theft.  
- **Fix:** Implement proper input validation and output encoding mechanisms.  

#### 📸 Proof of Concept

**Burp Suite Request (Payload Injection):**
![Burp Request](screenshots/xss-burp-request.PNG)

**Execution Confirmation:**
![XSS Execution](screenshots/xss-popup.PNG)

> Note: Execution was validated via application behavior (challenge completion), indicating successful payload processing.

---

### 2. SQL Injection (Basic)

- **Risk Level:** High  
- **Description:** The application failed to properly sanitize user input in database queries.  
- **Impact:** Attackers may gain unauthorized access to sensitive data or manipulate the database.  
- **Fix:** Use parameterized queries and prepared statements.  

#### 📸 Proof of Concept

![SQL Injection](screenshots/sqli-test.png)

---

### 3. Weak Authentication

- **Risk Level:** Medium  
- **Description:** The application allowed access using weak/default credentials.  
- **Impact:** Unauthorized users can gain access to restricted areas.  
- **Fix:** Enforce strong password policies and implement account lockout mechanisms.  

#### 📸 Proof of Concept

![Weak Authentication](screenshots/weak-auth.png)

---

## 📊 Key Learnings
- Hands-on experience with OWASP Top 10 vulnerabilities  
- Understanding of real-world attack and defense mechanisms  
- Practical usage of Burp Suite for request interception and analysis  
- Importance of secure coding practices  

---

## 🚀 Skills Demonstrated
- Web Application Security Testing (VAPT Basics)  
- Vulnerability Identification & Analysis  
- Manual Testing Techniques  
- Security Reporting & Documentation  

---

## ⚖️ Ethical Note
This project was conducted strictly in a controlled lab environment for educational purposes. No unauthorized systems were tested.
