 # Enterprise Information Security Risk Assessment & Treatment Plan
**Frameworks:** ISO/IEC 27005:2022 | ISO/IEC 27001:2022 Annex A | NIST SP 800-30 Rev 1  
**Author:** Bhavika Kothari (MSc Cyber Security & Digital Forensics)  
**Deliverable:** Interactive Executive Risk Register (`Enterprise_Risk_Register_ISO27005.xlsx`)

---

## 1. Project Overview & Scope
This project models an enterprise-level Information Security Risk Assessment for a Cloud & Managed Services Provider. It evaluates operational, technological, people, and third-party threat events across 10 critical organizational assets to determine **Inherent Risk**, map **ISO/IEC 27001:2022 controls**, and establish target **Residual Risk** thresholds.

---

## 2. Assessment Methodology
Risk scoring follows the standard $5 \times 5$ risk matrix ($Risk = Likelihood \times Impact$):
* **Likelihood Scale (1 to 5):** Rare (1), Unlikely (2), Possible (3), Likely (4), Almost Certain (5)
* **Impact Scale (1 to 5):** Negligible (1), Minor (2), Moderate (3), Major (4), Catastrophic (5)
* **Severity Thresholds:** Critical (15–25), High (10–14), Medium (6–9), Low (1–5)

---

## 3. Scenarios Evaluated
1. **Cloud DB (RSK-001):** Unpatched known CVEs $\rightarrow$ Mitigated via **ISO A.8.8** (Patch SLA < 7 days).
2. **Access Governance (RSK-002):** Delayed leaver deprovisioning $\rightarrow$ Mitigated via **ISO A.6.5** (ServiceNow SLA < 24 hrs).
3. **Third-Party Risk (RSK-003):** SaaS CRM vendor lacking SOC 2 $\rightarrow$ Mitigated via **ISO A.5.19** (TPRM questionnaire & encryption review).
4. **Endpoints (RSK-004):** Corporate laptops lacking encryption $\rightarrow$ Mitigated via **ISO A.8.1** (BitLocker MDM enforcement).
5. **Human Layer (RSK-005):** Spear-phishing & BEC attacks $\rightarrow$ Mitigated via **ISO A.6.3** (FIDO2 MFA & awareness simulations).
6. **Data Resilience (RSK-006):** Untested database restore drills $\rightarrow$ Mitigated via **ISO A.8.13** (Quarterly isolated staging drills).
7. **Web Applications (RSK-007):** SQLi & XSS flaws $\rightarrow$ Mitigated via **ISO A.8.25** (SAST/DAST automated code scanning).
8. **Logging & SIEM (RSK-008):** Inadequate firewall log retention $\rightarrow$ Mitigated via **ISO A.8.15** (365-day immutable cloud SIEM).
9. **Data Privacy (RSK-009):** Excessive PII retention $\rightarrow$ Mitigated via **ISO 27701** (Automated 3-year purge workflows).
10. **AI Governance (RSK-010):** Proprietary source code pasted into public LLMs $\rightarrow$ Mitigated via **ISO 42001** (Private enterprise LLM & DLP).

---

## 4. Key Results & Governance Impact
* **Total Risks Assessed:** 10
* **Initial Inherent Critical Risks:** 7 (Scores 15–25)
* **Residual Critical Risks Remaining:** **0** (All treated to Low or Medium acceptable thresholds)
* **Automated Features:** Nested `IF` rating formulas, Conditional Formatting risk heatmaps, Data Validation dropdowns, and executive `=COUNTIF()` KPI summary cards.
