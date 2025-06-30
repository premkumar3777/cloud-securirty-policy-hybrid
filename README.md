# 🔍 Cloud API Penetration Testing Report

This repository contains a penetration testing report for a cloud-based REST API. The test was conducted using **OWASP ZAP** to identify and remediate vulnerabilities before deployment of a startup's mobile app.

---

## 📋 Report Summary

The report includes:
- ✅ OWASP ZAP setup and configuration
- ✅ Target API description
- ✅ Scan results (active and passive)
- ✅ Identified vulnerabilities with remediation steps
- ✅ Final recommendations

---

## 🧪 Testing Setup

- **Tool**: OWASP ZAP (Zed Attack Proxy)
- **Platform**: Kali Linux VM
- **Proxy Configuration**: ZAP was configured to intercept and scan API calls
- **Target API**: Publicly available demo REST API simulating user login, registration, and data access

---

## 🚨 Key Findings

### 1. Insecure Direct Object Reference (IDOR)
- **Issue**: Access to other users' data by modifying user IDs in API requests
- **Fix**: Implement proper authorization checks for each object

### 2. SQL Injection
- **Issue**: Vulnerable query parameters in login endpoint
- **Fix**: Use prepared statements or parameterized queries with strict input validation

### 3. Excessive Data Exposure
- **Issue**: API responses included sensitive user metadata unnecessarily
- **Fix**: Minimize data returned to only what is required by the frontend

---

## ✅ Recommendations

- Apply the above mitigations before production deployment
- Integrate OWASP ZAP into the CI/CD pipeline for continuous testing
- Enable logging and monitoring for abnormal access patterns

---

## 📄 Download the Full Report

[📥 Download PDF](https://github.com/your-username/your-repo-name/blob/main/Cloud_API_Penetration_Test_Report.pdf)

> 🔁 Replace the link above with your actual GitHub path

---

## 📌 License

This report is intended for educational and internal security review purposes.
