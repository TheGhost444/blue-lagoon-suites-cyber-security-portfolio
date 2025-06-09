# AWS Cloud Security Controls – Blue Lagoon Suites

## Overview
Blue Lagoon Suites uses AWS to host the booking system, guest portal, and internal applications. The following controls help ensure security and compliance.

---

## 🔐 Identity & Access Management (IAM)

- Use **IAM roles** instead of long-term access keys
- Enable **MFA for root and IAM users**
- Apply **least privilege access** for all services

---

## ☁️ Data Security

- **S3 Buckets**: Encrypted using AES-256 (SSE-S3)
- **CloudTrail Logs**: Stored in a dedicated, immutable S3 bucket
- **RDS Encryption**: Enabled for all databases

---

## 🔒 Network Security

- Use **VPCs** with **private/public subnets**
- Restrict traffic using **Security Groups and NACLs**
- Enable **AWS Shield** for DDoS protection

---

## 🔁 Logging & Monitoring

- Enable **CloudTrail**, **Config**, and **GuardDuty**
- Use **AWS Config Rules** to monitor for misconfigurations
- Integrate with SIEM for alerting (Splunk, Sentinel, etc.)

---

## ✅ Compliance

- AWS environments monitored for PCI-DSS readiness
- Regular vulnerability scans via Inspector
- Backup compliance checked via AWS Backup Vault

---

## Recommendations

- Conduct regular IAM audits
- Set budget alerts to catch abuse
- Continuously scan AMIs for vulnerabilities before deployment
