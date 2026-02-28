# FUTURE-_CS_03# Task 3 – API Security Risk Analysis

## 📌 Overview
This project analyzes security risks in public APIs and identifies vulnerabilities related to authentication, authorization, data exposure, and input validation.

## 🎯 Objective
- Identify insecure API endpoints
- Analyze authentication & authorization mechanisms
- Detect missing rate limiting
- Evaluate input validation gaps
- Provide remediation strategies

## 🛠 Tools Used
- Postman
- Browser Developer Tools
- Sample Public APIs
- MS Word / Google Docs

## 🔍 Methodology
1. Collected API endpoints.
2. Tested authentication tokens.
3. Checked authorization controls.
4. Analyzed API responses for sensitive data.
5. Tested rate limiting and input validation.

## 🚨 Identified Risks

### 1. Broken Authentication (High)
- Missing or weak token validation.
- Risk: Unauthorized access.
- Fix: Implement JWT/OAuth with expiry.

### 2. Broken Authorization (High)
- No role verification.
- Risk: Access to other users’ data.
- Fix: Role-Based Access Control (RBAC).

### 3. Sensitive Data Exposure (High)
- API returns confidential data.
- Risk: Data breach.
- Fix: Encrypt & minimize response data.

### 4. No Rate Limiting (Medium)
- Unlimited API requests.
- Risk: DoS/Brute force.
- Fix: Apply request throttling.

### 5. Improper Input Validation (Medium)
- Accepts malicious input.
- Risk: Injection attacks.
- Fix: Input sanitization & validation.

## 📊 Risk Summary

| Risk | Severity | Impact |
|------|----------|--------|
| Broken Authentication | High | Unauthorized access |
| Broken Authorization | High | Data manipulation |
| Data Exposure | High | Privacy breach |
| No Rate Limiting | Medium | Service disruption |
| Poor Validation | Medium | Injection attacks |

## ✅ Conclusion
The API contains multiple security risks. Implementing authentication controls, rate limiting, encryption, and validation mechanisms will significantly improve security posture.

## 📚 References
- OWASP API Security Top 10
- API Security Best Practices
