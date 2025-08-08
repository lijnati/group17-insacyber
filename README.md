# 🔰 Web Application Firewall (WAF) 

##  Overview
The **Web Application Firewall (WAF)** is a security layer that sits between a client and a web application, filtering and blocking malicious HTTP requests before they reach the backend.  
Our WAF focuses on protecting against common vulnerabilities such as **SQL Injection (SQLi)**, **Cross-Site Scripting (XSS)**, and other injection attacks from the [OWASP Top 10](https://owasp.org/www-project-top-ten/).  

This project is built by **INSA summer camp cybersecurity department Group-17** as both a learning challenge and a practical demonstration of defensive security in action.



## Project Goals
- **Protect**: Intercept and block malicious requests.
- **Detect**: Identify attacks in real time using pattern matching and rules.
- **Educate**: Provide a hands-on security experience for the team.
- **Demonstrate**: Showcase the WAF blocking simulated attacks in a live environment.


## Key Features
- **HTTP Request Inspection** – Analyze query parameters, headers, and body content.
- **Attack Detection** – Regex-based rules for SQLi, XSS, and other common payloads.
- **Blocking Mechanism** – Automatically respond with `403 Forbidden` for malicious requests.
- **Customizable Rules Engine** – Update detection patterns without changing code.
- **Request Logging** – Record blocked attempts for forensic analysis.
- **IP Whitelisting/Blacklisting** – Control traffic sources.
- **Rate Limiting** – Reduce brute-force and flooding attempts.



## Architecture
```plaintext
Browser → WAF Layer → Web Server → Application → Database
