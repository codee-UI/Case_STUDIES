# Analyzing the Facebook and Google Phishing Case Study

**Estimated Duration:** 6 minutes  
**Topic:** Phishing, Social Engineering, Email Spoofing, Fraud Prevention, and Incident Response

---

## 1. Introduction

The phishing attack targeting Facebook and Google between 2013 and 2015 demonstrates how sophisticated social engineering attacks can exploit weaknesses in the financial processes of even large technology organizations.

Evaldas Rimasauskas impersonated a legitimate business partner, Quanta Computer, by establishing a fraudulent company and sending fake invoices and payment requests. By exploiting trust in established business relationships and weaknesses in invoice verification procedures, he defrauded the companies of approximately $100 million.

This case study highlights the importance of robust financial verification procedures, employee awareness, effective incident detection, and strong cybersecurity controls.

## 2. Case Study Overview

| Attribute | Details |
|---|---|
| Incident type | Business Email Compromise (BEC) and payment fraud |
| Primary techniques | Social engineering, impersonation, fraudulent invoices, and deceptive payment instructions |
| Attacker | Evaldas Rimasauskas |
| Target organizations | Facebook and Google |
| Incident period | 2013–2015 |
| Reported amount | Approximately $100 million |
| Primary vulnerability | Weaknesses in vendor verification and payment authorization processes |
| Main lesson | Independently verify vendors, invoices, and changes to payment instructions |

## 3. Root Cause Analysis

### 3.1 Initial Point of Failure

The attacker exploited weaknesses in the organizations' financial workflows by impersonating Quanta Computer, a legitimate Taiwanese electronics manufacturer that had business relationships with the targeted companies.

He established a fraudulent company and used deceptive documentation and communications to make fraudulent invoices and payment requests appear legitimate.

The primary failure was insufficient verification of the authenticity of the vendor and the payment instructions.

### 3.2 Contributing Factors

**1. Inadequate verification mechanisms**

Weak vendor onboarding, invoice validation, and payment authorization procedures can allow fraudulent requests to pass through legitimate financial workflows.

**2. Social engineering**

The attacker exploited employee trust in an established supplier relationship and used communications that appeared consistent with normal business operations.

**3. Email impersonation and deceptive communications**

Fraudulent communications can make payment requests appear to originate from legitimate business partners. Email authentication controls alone cannot prevent every form of business email compromise.

**4. Insufficient separation of duties**

If a single employee can approve a vendor, validate an invoice, and authorize a payment, fraudulent transactions may be more difficult to detect.

**5. Limited transaction anomaly detection**

Unusual payment destinations, changes in bank details, unexpected invoice patterns, or deviations from normal transaction behavior can indicate fraud and should trigger additional review.

## 4. Evaluate Effectiveness and Timeliness

### Initial Detection

The fraudulent payments continued over an extended period, demonstrating that preventive controls and early detection mechanisms were insufficient to identify the scheme promptly.

### Response After Discovery

Once the fraud was discovered, the organizations cooperated with law enforcement and pursued recovery of funds. The investigation demonstrated the importance of preserving financial records, tracing transactions, and coordinating with relevant authorities.

### Overall Assessment

The incident illustrates a distinction between **prevention, detection, and response**. Effective incident response can limit damage after discovery, but it cannot replace strong preventive controls and continuous monitoring.

## 5. Successes, Gaps, and Failures

### Successes

- The fraudulent activity was eventually identified and investigated.
- Cooperation with law enforcement supported the investigation and prosecution.
- The case demonstrated the value of financial transaction records and cross-organizational cooperation.

### Security Gaps

- Vendor identity and payment instructions were not adequately verified.
- Fraudulent invoices were able to pass through established payment workflows.
- Existing controls did not detect the suspicious activity early enough.
- Financial processes required stronger independent review and transaction monitoring.

### Key Failures

The central failure was not simply that employees received deceptive communications. It was that the attacker could exploit business processes to convert those communications into unauthorized payments.

Security controls must therefore address both human behavior and the technical and procedural systems used to authorize financial transactions.

## 6. Impact on the Organizations

### Financial Impact

The scheme involved approximately $100 million in fraudulent payments. Financial fraud can also create additional costs associated with investigation, recovery efforts, and control improvements.

### Operational Impact

The organizations needed to investigate the incident, review financial transactions, coordinate internally, and strengthen their payment controls.

### Legal and Reputational Impact

The incident required cooperation with law enforcement and highlighted the potential reputational consequences of weaknesses in financial security processes.

### Organizational Learning

The case demonstrated that organizational size, technical expertise, and substantial cybersecurity resources do not eliminate the risk of fraud through legitimate business workflows.

## 7. Lessons Learned

### 7.1 Verify Vendors Independently

Organizations should validate new vendors using trusted, independently obtained contact information. Changes to supplier bank accounts or payment instructions should be verified through a separate, previously established communication channel.

### 7.2 Strengthen Payment Authorization

Financial transactions should require appropriate authorization based on their risk and value. High-value payments and changes to payment details should receive additional independent review.

### 7.3 Improve Employee Awareness

Employees should learn to recognize impersonation, unexpected payment requests, urgency, unusual invoice details, and suspicious changes to supplier information.

### 7.4 Apply Separation of Duties

Vendor registration, invoice approval, and payment execution should be separated where practical. No single individual should have unrestricted control over the entire payment process.

### 7.5 Monitor Financial Transactions

Organizations should monitor for unusual transaction amounts, unexpected payment destinations, duplicate invoices, abnormal vendor activity, and changes that deviate from established business patterns.

### 7.6 Maintain Incident Response Procedures

Organizations should have documented procedures for reporting suspected fraud, preserving evidence, contacting financial institutions, investigating transactions, and notifying law enforcement when appropriate.

## 8. Recommendations for Future Actions

| Recommendation | Implementation | Expected Benefit |
|---|---|---|
| Independent vendor verification | Validate vendor identities using trusted contact details | Reduces impersonation risk |
| Multi-person payment approval | Require independent approval for high-risk transactions | Prevents unauthorized payments |
| Employee security training | Conduct regular phishing and BEC awareness exercises | Improves recognition and reporting |
| Email security controls | Configure SPF, DKIM, and DMARC appropriately | Helps reduce certain forms of email spoofing |
| Financial anomaly detection | Flag unusual payment amounts, destinations, and invoice patterns | Supports earlier fraud detection |
| Separation of duties | Separate vendor creation, invoice approval, and payment execution | Reduces opportunities for internal process abuse |
| Incident response planning | Establish reporting, investigation, and recovery procedures | Improves response speed and consistency |
| Periodic control audits | Review vendor records, payment approvals, and exceptions | Identifies control weaknesses before exploitation |

**Important:** SPF, DKIM, and DMARC are useful email security controls, but they do not independently prevent all impersonation or business email compromise attacks.

## 9. Role of AI and Machine Learning in Fraud Detection

AI and machine learning can complement traditional financial controls by identifying unusual patterns in invoices, vendor behavior, and payment transactions.

Potential applications include:

- **Anomaly detection:** Identify transactions that differ significantly from normal payment behavior.
- **Duplicate invoice detection:** Flag repeated invoice numbers, amounts, or suspiciously similar documents.
- **Vendor behavior analysis:** Detect unexpected changes in payment destinations or transaction frequency.
- **Email classification:** Identify suspicious messages using sender information, message content, and contextual indicators.
- **Risk scoring:** Prioritize transactions for manual review according to their estimated fraud risk.

AI systems should support, rather than replace, independent verification and human authorization. False positives, manipulated inputs, and incomplete training data must also be considered.

## 10. Incident Prevention Workflow

```text
Vendor Registration
        |
        v
Independent Vendor Verification
        |
        v
Invoice and Purchase Order Matching
        |
        v
Payment Risk Assessment
        |
        v
Independent Authorization
        |
        v
Payment Execution
        |
        v
Continuous Transaction Monitoring
        |
        v
Suspicious Activity Detected?
        |
   +----+----+
   |         |
  No        Yes
   |         |
   v         v
Continue   Hold or Review
Monitoring    |
              v
       Investigate and Preserve Evidence
              |
              v
       Notify Relevant Parties
              |
              v
       Recover Funds and Improve Controls
```

## 11. Conclusion

The Facebook and Google phishing case demonstrates how business email compromise, social engineering, and inadequate financial verification can result in substantial financial losses. The attack exploited trust in a legitimate supplier relationship and weaknesses in payment authorization processes.

Organizations can reduce similar risks by independently verifying vendors and payment changes, enforcing separation of duties, training employees, monitoring financial transactions, and maintaining effective incident response procedures. AI and machine learning can provide additional detection capabilities, but they should complement strong governance and established financial controls.

The most important lesson is that cybersecurity must protect not only computer systems and networks but also the business processes through which attackers can cause harm.

## 12. Quick Revision Notes

- **Attack type:** Business Email Compromise (BEC) and payment fraud.
- **Primary techniques:** Social engineering, supplier impersonation, fraudulent invoices, and deceptive payment instructions.
- **Root cause:** Inadequate verification and payment controls.
- **Primary preventive control:** Independently verify vendor identities and payment changes.
- **Important administrative controls:** Separation of duties and multi-person authorization.
- **Important technical controls:** Email authentication, transaction monitoring, and anomaly detection.
- **Incident response priorities:** Investigate, preserve evidence, contact relevant financial institutions, and cooperate with law enforcement.
- **AI/ML application:** Detect anomalous transactions and prioritize suspicious activity for investigation.

---

**End of Study Notes**