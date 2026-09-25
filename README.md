# Web Application Firewall (WAF) Implementation Project

This project demonstrates the deployment and configuration of a Web Application Firewall (WAF) to secure a modern, intentionally vulnerable web application, OWASP Juice Shop[span_1](start_span)[span_1](end_span). 

## 🛡️ Project Overview
* **Target Application:** OWASP Juice Shop[span_2](start_span)[span_2](end_span)
* **Security Component:** ModSecurity WAF with OWASP Core Rule Set (CRS)[span_3](start_span)[span_3](end_span)
* **Operating System:** Kali Linux[span_4](start_span)[span_4](end_span)
* **Containerization:** Docker & Docker Compose[span_5](start_span)[span_5](end_span)
* **Submitted By:** Irfan A[span_6](start_span)[span_6](end_span)

## 🚀 Objectives
* Deploy OWASP Juice Shop as an isolated vulnerable environment using Docker[span_7](start_span)[span_7](end_span).
* Configure ModSecurity as an inline protection layer (reverse proxy via Nginx)[span_8](start_span)[span_8](end_span).
* Simulate and block common web attacks such as SQL Injection (SQLi), Cross-Site Scripting (XSS), and Command Injection[span_9](start_span)[span_9](end_span).
* Validate WAF performance using automated testing scripts and analyze forensic logs[span_10](start_span)[span_10](end_span).

## 🧪 Testing Results
The automated WAF testing script (`test-waf.sh`) achieved a **100% pass rate**, successfully blocking all malicious exploit payloads with a `403 Forbidden` response while allowing legitimate traffic (`200 OK`) to pass through[span_11](start_span)[span_11](end_span).

* **SQL Injection Tests:** Blocked (403)[span_12](start_span)[span_12](end_span)
* **XSS Tests:** Blocked (403)[span_13](start_span)[span_13](end_span)
* **Command Injection & Path Traversal:** Blocked (403)[span_14](start_span)[span_14](end_span)
* **Normal Traffic:** Allowed (200)[span_15](start_span)[span_15](end_span)

## 📁 Repository Structure
* `docker-compose.yml`: Configuration file for deploying Juice Shop and ModSecurity WAF containers[span_16](start_span)[span_16](end_span).
* `test-waf.sh`: Automated bash script used to test various attack vectors and normal traffic[span_17](start_span)[span_17](end_span).
* `logs/`: Contains audit trails and evidence of blocked attacks[span_18](start_span)[span_18](end_span).
* `WEB APPLICATION FIREWALL impliment project.pdf`: Detailed project report[span_19](start_span)[span_19](end_span).
