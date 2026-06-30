# Security Audit & Risk Assessment Report: Botium Toys (Fictional company)

## 📌 Project Overview
This project consists of a comprehensive security audit and risk assessment conducted for **Botium Toys**. The primary objective was to evaluate the organization's existing infrastructure, identify security vulnerabilities, and assess compliance against industry standards such as **NIST CSF**, **PCI DSS**, and **GDPR**. 

Based on the findings, a strategic roadmap and technical recommendations were developed to harden Botium Toys' overall security posture.

---

## 🎯 Scope & Goals
* **Scope:** The entire security program at Botium Toys, including internal networks, systems, on-premises equipment, employee end-user devices, and legacy infrastructure.
* **Goals:** Assess existing assets, complete a controls and compliance checklist, determine gaps in the current security posture, and provide actionable remediation steps.

---

## 📊 Risk Assessment Summary
* **Risk Score:** `8 / 10` (High Risk)
* **Risk Description:** Inadequate asset management, lack of essential technical controls, absence of disaster recovery/backup strategies, and partial non-compliance with international regulatory data privacy standards.

---

## 🛠️ Controls Assessment Checklist
Below is the status of security controls audited during this assessment:

| Control Type | Implemented? | Notes |
| :--- | :---: | :--- |
| **Firewall** | ✅ Yes | Restricts traffic based on defined security rules. |
| **Antivirus Software** | ✅ Yes | Installed and monitored regularly by the IT department. |
| **Manual Legacy Monitoring** | ✅ Yes | Monitored manually, but lacks a regular maintenance schedule. |
| **Physical Security (Locks/CCTV)** | ✅ Yes | Sufficient locks, up-to-date CCTV, and functioning fire prevention. |
| **Least Privilege / RBAC** | ❌ No | All employees have unrestricted access to internal and sensitive data. |
| **Separation of Duties** | ❌ No | Not implemented; creates significant insider risk. |
| **Encryption** | ❌ No | Customer cardholder data and PII/SPII are stored locally in plaintext. |
| **Intrusion Detection System (IDS)** | ❌ No | The internal network lacks automated threat detection capabilities. |
| **Backups & Disaster Recovery** | ❌ No | No data backups or Disaster Recovery Plans (DRP) currently exist. |
| **Password Management System** | ❌ No | Nominal password requirements; lacks centralized enforcement. |

---

## ⚖️ Compliance Assessment Gaps
* **PCI DSS:** **Non-Compliant**. Unencrypted cardholder data is stored locally, and access is not restricted to authorized users.
* **GDPR:** **Partially Compliant**. Privacy policies are enforced, and a 72-hour breach notification plan exists for E.U. citizens; however, sensitive user data lacks appropriate confidentiality safeguards (encryption).
* **SOC (Type 1 / Type 2):** **Non-Compliant**. User access policies are weak, and PII/SPII data privacy is not properly maintained.

---

## 💡 Strategic Recommendations

1. **Access Control & Privilege Management**
   * Implement **Role-Based Access Control (RBAC)** based on the **Principle of Least Privilege** and **Separation of Duties** to restrict unauthorized employee access to sensitive cardholder data.

2. **Data Protection & Encryption**
   * Enforce strong encryption (**AES-256**) for all PII/SPII and financial data both **at rest and in transit**. Strictly prohibit the unsecured local storage of plaintext credit card information to achieve **PCI DSS compliance**.

3. **Network Security & Threat Detection**
   * Deploy a centralized **Intrusion Detection System (IDS)** to monitor internal network traffic and proactively identify anomalous behavior or potential lateral movement.

4. **Business Continuity & Disaster Recovery**
   * Develop a comprehensive **Disaster Recovery Plan (DRP)** and implement an automated, regularly tested backup schedule (adhering to a **3-2-1 backup strategy**) to guarantee data availability.

5. **Identity & Password Hardening**
   * Upgrade the corporate password policy complexity requirements (minimum length, special characters, numbers) and deploy a **Centralized Password Management System** to streamline operations and enforce compliance.

6. **Lifecycle & Lifecycle Management**
   * Establish a formal schedule for the maintenance, monitoring, and eventual decommissioning or isolation of **End-of-Life (EOL) legacy systems** to mitigate unpatched exploit risks.

---

## 📁 Repository Structure
* `README.md` - Executive summary and project documentation (this file).
* `Botium_Toys_Security_Audit_Report.pdf` - The final comprehensive PDF report containing detailed checklists and risk metrics.
* `Botium Toys_ Scope, goals, and risk assessment report.pdf` - The risk assessment report PDF.
