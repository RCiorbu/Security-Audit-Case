# Cybersecurity Audit Case Study 
## Objective 
Perform a security audit on a simulated organization using a provided checklist. 
Identify strengths, weaknesses, and provide recommendations.
## Case Scenario: Botium Toys Security Audit
## Scope
The audit covers Botium Toys’ overall security program, including employee equipment, internal networks, systems, data storage, and storefront operations (online and in-person).
## Goals
- Assess existing assets and controls.
- Complete the compliance checklist.
- Recommend improvements to strengthen security posture.

## Current Assets
- On-premises business equipment (computers, smartphones, remote devices, cameras).
- Storefront and warehouse products.
- Internal systems (accounting, telecom, database, ecommerce, inventory).
- Internet access, internal network, data retention/storage.
- Legacy systems requiring manual monitoring.

## Risk Assessment
- **Key risks**: Inadequate asset management, lack of encryption, weak access controls, no IDS, and no disaster recovery plans.  
- **Strengths**: Firewall and antivirus are in place; physical security (locks, CCTV, fire detection) is adequate.  
- **Risk score**: 8/10 (high).

## Notable Issues
- Employees have broad access to sensitive customer data,  (including payment info).
- No encryption for credit card data stored in the internal database.
- Weak password policy; no centralized password management.
- No backups of critical data or disaster recovery plan.
- Legacy system maintenance lacks a clear schedule.

# Controls Assessment Checklist – Botium Toys

## General Security Controls

| Control                                             | Status |
|-----------------------------------------------------|--------|
| Least Privilege                                     | ❌ No  |
| Disaster Recovery Plans                             | ❌ No  |
| Password Policies                                   | ❌ No (weak policy in place) |
| Separation of Duties                                | ❌ No  |
| Firewall                                            | ✅ Yes |
| Intrusion Detection System (IDS)                    | ❌ No  |
| Backups                                             | ❌ No  |
| Antivirus Software                                  | ✅ Yes |
| Legacy Systems Monitoring & Maintenance             | ❌ No (ad-hoc only) |
| Encryption                                          | ❌ No  |
| Password Management System                          | ❌ No  |
| Locks (offices, storefront, warehouse)              | ✅ Yes |
| Closed-Circuit Television (CCTV)                    | ✅ Yes |
| Fire Detection/Prevention (alarms, sprinklers, etc.)| ✅ Yes |

---

## Compliance Checklist

### Payment Card Industry Data Security Standard (PCI DSS)

| Best Practice | Status |
|---------------|--------|
| Only authorized users have access to customers’ credit card info | ❌ No |
| Credit card info stored/processed/transmitted securely | ❌ No |
| Data encryption procedures in place | ❌ No |
| Secure password management policies | ❌ No |

---

### General Data Protection Regulation (GDPR)

| Best Practice | Status |
|---------------|--------|
| E.U. customers’ data is kept private/secure | ❌ No |
| Breach notification plan within 72 hours | ✅ Yes |
| Data properly classified and inventoried | ❌ No |
| Privacy policies/procedures enforced | ✅ Yes |

---

### System and Organization Controls (SOC 1 & SOC 2)

| Best Practice | Status |
|---------------|--------|
| User access policies established | ❌ No |
| Sensitive data (PII/SPII) remains confidential | ❌ No |
| Data integrity (accurate, validated, complete) | ✅ Yes |
| Data available to authorized users only | ❌ No |

---

## Recommendations
- Implement least privilege and separation of duties immediately to reduce insider threat risks.  
- Develop and test a disaster recovery plan, including regular backups of critical systems.  
- Enforce stronger password policies and adopt a centralized password management system.  
- Encrypt all sensitive and financial data (PCI DSS requirement).  
- Deploy an intrusion detection system (IDS) for real-time monitoring.  
- Improve data classification and inventory to support GDPR and SOC compliance.

# Audit Findings Report – Botium Toys

## Overview
This report summarizes the results of a security audit conducted on Botium Toys.  
The audit assessed technical controls, compliance practices, and overall risk posture using the provided checklist.

## Strengths
- **Firewall** is properly configured with defined security rules.  
- **Antivirus software** is installed and monitored by the IT department.  
- **Physical security** is adequate, including locks, CCTV surveillance, and fire detection/prevention systems.  
- **EU breach notification plan** is established to notify customers within 72 hours of a security incident.  
- **Data integrity controls** are in place to maintain consistency and accuracy.  
- **Privacy policies and procedures** exist and are enforced within the IT department.  

## Weaknesses
- **No encryption** is in place to protect customer credit card data (PCI DSS violation).  
- **Excessive access**: All employees can access sensitive data, including customer PII/SPII.  
- **No intrusion detection system (IDS)** to monitor and respond to threats in real time.  
- **No backups or disaster recovery plan**, placing business continuity at high risk.  
- **Weak password policy** and **no centralized password management system**, leading to poor credential security.  
- **Least privilege and separation of duties not implemented**, creating insider threat risks.  
- **Legacy systems** are monitored inconsistently, with unclear intervention processes.  
- **Data classification and inventory** processes are missing, hindering GDPR and SOC compliance.  

## Risk Score
**8/10 (High)** — Due to the absence of critical controls (encryption, backups, IDS) and non-compliance with PCI DSS, GDPR, and SOC frameworks.  

## Recommendations
1. **Implement Data Encryption**  
   - Encrypt customer financial and sensitive data to comply with PCI DSS and GDPR requirements.  

2. **Restrict Access with Least Privilege**  
   - Assign role-based access controls to limit exposure of customer PII/SPII.  

3. **Deploy an IDS and SIEM Solution**  
   - Implement monitoring tools to detect suspicious activity and generate alerts.  

4. **Develop a Disaster Recovery & Backup Plan**  
   - Establish regular backups of critical systems and test disaster recovery procedures.  

5. **Strengthen Password Security**  
   - Update password policy to meet NIST standards (minimum length, complexity, expiration).  
   - Introduce a centralized password management system.  

6. **Enhance Governance and Compliance**  
   - Inventory and classify data to improve GDPR and SOC compliance.  
   - Enforce separation of duties to reduce internal risks.  

7. **Formalize Legacy System Management**  
   - Create a documented schedule and intervention plan for legacy system maintenance.  

## Conclusion
Botium Toys has a solid foundation in **physical security and basic IT controls**, but significant gaps remain in **data security, compliance, and disaster preparedness**. Addressing the weaknesses outlined above will greatly reduce the company’s exposure to risks, improve regulatory compliance, and strengthen overall security posture.
