# Course 2 | Portfolio Activity: Conducting a Security Audit

---

## Overview

The goal of this portfolio activity was to become familiar with conducting an internal security audit for 
a company. A fictional company Botium Toys was used as a case study in the Google
Cybersecurity Professional Certificate. This audit was based on a provided
scope, goals, and risk assessment report, with the objective of identifying
gaps in controls and compliance that could expose the company to risk. An optional objective was to recommend
specific controls and frameworks as well as devise a plan to communicate to stakeholders on how to reduce the company's risk to assets
and improve security posture.

---

## Frameworks & Principles Applied

- **NIST Cybersecurity Framework (CSF)**
- **CIA Triad** (Confidentiality, Integrity, Availability)
- **OWASP Security Principles**

## Audit Scope

The audit evaluated Botium Toys' adherence to the following compliance
frameworks:

- Payment Card Industry Data Security Standard (PCI DSS)
- General Data Protection Regulation (GDPR)
- System and Organization Controls (SOC type 1, SOC type 2)

## Key Findings

**PCI DSS** -- Significant gaps were identified including unauthorized access to customer
credit card information not restricted, encryption procedures for
transaction data not implemented, and secure password management
policies not in place. Only internal processing of card data in a
secure environment was confirmed.

**GDPR** -- Partial compliance. A breach notification plan within the 72-hour
window and enforced privacy policies were in place; however, EU customer
data was not adequately secured and data classification/inventory procedures
were absent.

**SOC 1 / SOC 2** -- Mixed results. Data integrity controls were in place,
but user access policies and confidentiality of sensitive PII/SPII were
not established.

## Recommendations

Priority controls to implement to reduce risk and improve Botium Toys'
security posture:

- Enforce least privilege and separation of duties across all employees
- Implement data encryption for all sensitive and financial data
- Deploy an intrusion detection system (IDS)
- Establish a centralized password management system with stronger policies
- Create and test disaster recovery plans and data backups immediately

## Reflection: Comparison with Exemplar

After completing the audit, I reviewed the provided exemplar answer to
identify areas where my assessment differed.

**Password Policies -- I marked Yes; exemplar marked No.**
The risk assessment noted that employee password requirements were minimal.
I interpreted the existence of any password policy as a partial control in
place, but the exemplar correctly identifies that minimal/nominal policies
do not constitute an adequate control. This was a good reminder that the
*quality* of a control matters as much as its presence — a weak password
policy provides little real protection and should not be counted as
compliant.

**Manual Monitoring for Legacy Systems -- I marked Yes; exemplar marked No.**
The risk assessment mentioned that legacy systems are monitored and
maintained, which led me to mark this as in place. However, the exemplar
flags that without a regular schedule or clear intervention procedures,
this does not qualify as a proper control. This distinction highlights the
importance of evaluating whether a control is consistently and formally
implemented, not just informally practiced.

**PCI DSS -- Secure environment for card processing - I marked Yes; exemplar
marked No.**
I noted that credit card information is processed internally, which I
interpreted as a secure environment. The exemplar clarifies that because
card data is unencrypted and accessible to all employees, it cannot be
considered a secure environment. This reinforced the principle that security
controls must be evaluated holistically -- internal processing alone does not
satisfy the requirement without accompanying access controls and encryption.

These discrepancies reflect a common challenge in real-world auditing:
distinguishing between controls that technically exist and controls that are
effectively implemented. Going forward, I will apply a stricter standard
when assessing control adequacy and definitively flag controls as inadequate. 

## Files

- `Controls_and_compliance_checklist.pdf` — My completed audit checklist
- `Controls_and_compliance_checklist_exemplar.pdf` — Google-provided
  exemplar for comparison
- `Botium_Toys_Scope_Goals_Risk_Assessment.pdf` — Source risk assessment
  report
