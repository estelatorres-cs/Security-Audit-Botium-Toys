# Security Audit for Botium Toys  

## 📝 Overview  
This repository contains the findings, risk assessment, and recommendations from a security audit conducted for **Botium Toys**. The goal of this audit was to assess existing assets, determine security vulnerabilities, and provide recommendations to improve the overall security posture of the organization.  

## 🔍 Audit Scope & Goals  
### **Scope:**  
The audit covers the entire security program at Botium Toys, including:  
- Employee equipment (desktops, laptops, smartphones, etc.)  
- Internal network and systems  
- Management of software and services (accounting, telecommunication, ecommerce, inventory)  
- Internet access, data retention, and storage  
- Legacy system maintenance  

### **Goals:**  
The primary goal is to evaluate the existing security controls and compliance measures in place and identify best practices that need to be implemented to enhance Botium Toys’ security framework.  

## 🛠️ Risk Assessment & Findings  
### **Risk Description:**  
There is inadequate management of assets, and Botium Toys is not fully compliant with U.S. and international standards and regulations. This includes gaps in security controls, which could lead to data breaches or other risks.  

### **Control Best Practices:**  
The **NIST Cybersecurity Framework (CSF)** was used for assessing the controls. Specifically, the first function, **Identify**, was a key focus. Asset classification and risk identification were prioritized to mitigate risks associated with business continuity.

### **Risk Score:**  
The current risk score is **8/10**, which reflects a fairly high risk due to missing security controls and inadequate adherence to compliance standards.  

### **Additional Comments:**  
- All employees have unrestricted access to internal data, including sensitive customer information like PII/SPII and credit card details.  
- Encryption is not used for sensitive data, including credit card information.  
- Key security measures like **least privilege access**, **separation of duties**, and **intrusion detection** are not in place.  
- The company does not have disaster recovery plans or proper data backup practices.  
- There is no centralized **password management system** or strong password policies.

## 📑 Findings & Controls Checklist  

### **Security Controls:**  
| **Control** | **Implemented** |  
|-------------|-----------------|  
| Least Privilege | No |  
| Disaster Recovery Plans | No |  
| Password Policies | No |  
| Separation of Duties | No |  
| Firewall | Yes |  
| Intrusion Detection System (IDS) | No |  
| Backups | No |  
| Antivirus Software | Yes |  
| Legacy System Maintenance | No |  
| Encryption | No |  
| Password Management System | No |  
| Physical Security (Locks, CCTV) | Yes |  
| Fire Detection/Prevention | Yes |  

### **Compliance Checklist:**  
#### **PCI-DSS (Payment Card Industry Data Security Standard)**  
- Only authorized users have access to credit card data: **No**  
- Credit card data is securely stored and processed: **No**  
- Data encryption procedures implemented: **No**  
- Secure password management: **No**  

#### **GDPR (General Data Protection Regulation)**  
- E.U. customer data is private/secure: **No**  
- Breach notification plan in place: **Yes** (within 72 hours)  
- Data classification and inventory: **No**  
- Privacy policies enforced: **Yes**  

#### **SOC (System and Organizations Controls)**  
- User access policies established: **No**  
- Sensitive data (PII/SPII) is confidential: **No**  
- Data integrity is ensured: **Yes**  
- Data is accessible to authorized users: **Yes**  

## 🔐 Recommendations  
### **1. Implement Data Encryption:**  
- **Action:** Encrypt sensitive data (e.g., credit card info, PII) at rest and in transit using AES-256 for storage and TLS for transmission.  
- **Compliance Benefit:** PCI-DSS and GDPR compliance.

### **2. Access Controls - Least Privilege & Separation of Duties:**  
- **Action:** Implement **role-based access control (RBAC)** to ensure employees only have access to necessary data.  
- **Compliance Benefit:** Mitigates internal risks and aligns with **NIST** and **GDPR**.

### **3. Install an Intrusion Detection System (IDS):**  
- **Action:** Deploy an IDS (e.g., Snort or Suricata) to monitor network activity for suspicious behavior.  
- **Compliance Benefit:** Helps protect assets and meets security expectations in **ISO 27001** and **NIST** frameworks.

### **4. Disaster Recovery Plan and Backups:**  
- **Action:** Develop a **disaster recovery plan** and establish regular data backup practices.  
- **Compliance Benefit:** Ensures business continuity and meets **GDPR** and **PCI-DSS** requirements.

### **5. Strengthen Password Policies:**  
- **Action:** Enhance password complexity requirements and implement a **centralized password management system**.  
- **Compliance Benefit:** Aligns with **NIST SP 800-63** for password security.

### **6. Regular Maintenance for Legacy Systems:**  
- **Action:** Schedule regular updates and vulnerability assessments for legacy systems.  
- **Compliance Benefit:** Reduces vulnerabilities and follows **CIS Controls** and **NIST** guidelines.

### **7. Enhanced Security Monitoring & Logging:**  
- **Action:** Centralize logging and enable real-time alerts for access to sensitive data.  
- **Compliance Benefit:** Meets security auditing requirements for **GDPR**, **ISO 27001**, and **PCI-DSS**.

### **8. Improve Physical Security:**  
- **Action:** Consider access control systems and conduct regular security drills.  
- **Compliance Benefit:** Aligns with **PCI-DSS** and **ISO 27001** standards for physical security.

### **9. Staff Training & Awareness:**  
- **Action:** Provide regular cybersecurity awareness training.  
- **Compliance Benefit:** Reduces human error and enhances compliance with **GDPR** and other regulations.

### **10. Breach Notification Procedures:**  
- **Action:** Ensure breach notification procedures meet regulatory timelines (72-hour GDPR rule).  
- **Compliance Benefit:** Ensures transparency and compliance with **GDPR**.

---

## 📥 Conclusion  
By implementing these recommended actions, **Botium Toys** can improve its security posture, reduce potential vulnerabilities, and align with relevant security standards and regulations like **PCI-DSS**, **GDPR**, and **ISO 27001**.  
