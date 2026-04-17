# Controls Implementation Plan — Phase 2 Gap Remediation
**Document Type:** Controls Tracking  
**Classification:** Internal - Restricted  
**Systems Covered:** NP-001 Credit Scoring Engine · NP-002 Fraud Detection System  
**Source:** Phase 2 AI Risk Assessment findings  
**Owner:** AI Governance Programme Office  
**Status:** 🟡 In Progress - Q2/Q3 2025 target  


---

## Purpose

This document translates the seven compliance gaps identified in the Phase 2 AI Risk Assessment into a tracked controls implementation plan. Each gap is assigned a specific control, a named owner, a target completion date and a success criterion.

This plan is reviewed monthly by the AI Governance Programme Office and reported quarterly to the AI Governance Committee until all controls reach green status.

---

## Background

Phase 2 of NorthPoint's AI Governance Programme completed a full risk assessment of the two HIGH RISK systems in the portfolio. The Article 9 compliance review identified seven gaps - two non-compliant requirements for NP-001 and two partial gaps for NP-002.

The gaps by system:

**NP-001 Credit Scoring Engine (5 gaps):**
- Bias testing not yet commissioned (NON-COMPLIANT)
- Explainability layer not implemented (NON-COMPLIANT)
- Review schedule not formalised in governance calendar (PARTIAL)
- Monitoring to risk register feedback loop not established (PARTIAL)
- Fairness metrics and thresholds not defined (PARTIAL)

**NP-002 Fraud Detection System (2 gaps):**
- Robustness testing schedule not formalised (PARTIAL)
- False positive SLA not defined or monitored (PARTIAL)

---

## Controls Implementation Tracker

---

### CTRL-001 — Independent Bias Audit for NP-001

| Field | Detail |
|---|---|
| **Control ID** | CTRL-001 |
| **Source Gap** | Phase 2 - GAP-03: Bias testing not commissioned (NON-COMPLIANT) |
| **System** | NP-001 Credit Scoring Engine |
| **Regulatory Reference** | EU AI Act Articles 9 and 10; UK Equality Act 2010 |
| **Risk Addressed** | RISK-NP001-01 (Demographic bias - Critical) and RISK-NP001-03 (Historical training data bias - High) |
| **Control Description** | Commission an independent third-party disparate impact audit of the Credit Scoring Engine across all relevant protected characteristics: race/ethnicity, gender, age and disability. The audit uses Article 10(5) exemption to access sensitive demographic data for bias detection purposes only. |
| **Owner** | Head of Credit Risk |
| **Target Completion** | Q2 2025 |
| **Estimated Cost** | £40,000 - £80,000 |
| **Status** | 🟡 In Progress |

**Success Criteria:**
- Independent audit firm engaged and audit scope agreed
- Disparate impact analysis completed across all four protected characteristic groups
- Audit findings documented in a formal report and shared with the AI Governance Committee
- Remediation actions identified for any confirmed disparate impact

**Implementation Steps:**

| Step | Action | Owner | Due |
|---|---|---|---|
| 1 | Issue RFP to minimum three specialist AI audit firms | AGPO | Month 1 |
| 2 | Select audit provider and agree scope | Head of Credit Risk | Month 1 |
| 3 | Invoke Article 10(5) exemption - document legal basis for sensitive data access | DPO | Month 1 |
| 4 | Provide audit firm with model access, training data and system documentation | ML Engineering | Month 2 |
| 5 | Audit firm conducts disparate impact analysis | External Auditor | Months 2-3 |
| 6 | Review draft findings and agree final report | Head of Credit Risk | Month 3 |
| 7 | Present findings to AI Governance Committee | AGPO | Month 3 |
| 8 | Initiate remediation for any confirmed disparate impact | Head of Credit Risk | Month 4+ |

**Interim Control:** Pending audit completion, a manual review pathway is in place for credit refusals where the applicant profile indicates elevated bias risk (thin-file applicants and postcodes with high protected characteristic correlation).

---

### CTRL-002 — Explainability Layer for NP-001

| Field | Detail |
|---|---|
| **Control ID** | CTRL-002 |
| **Source Gap** | Phase 2 - GAP-04: Explainability layer not implemented (NON-COMPLIANT) |
| **System** | NP-001 Credit Scoring Engine |
| **Regulatory Reference** | EU AI Act Article 13; GDPR Article 22; FCA Consumer Duty |
| **Risk Addressed** | RISK-NP001-02 (Lack of explainability for credit refusals - High) |
| **Control Description** | Implement a SHAP (SHapley Additive exPlanations) post-hoc explainability layer on NP-001 model outputs. Develop customer-facing refusal communication templates presenting the top three contributing factors in plain language. Train customer service staff on communicating credit decision explanations. |
| **Owner** | Head of Credit Risk |
| **Target Completion** | Q2 2025 |
| **Estimated Cost** | £15,000 - £25,000 |
| **Status** | 🟡 In Progress |

**Success Criteria:**
- SHAP explainability layer implemented and generating factor-level outputs for every decision
- Customer refusal letter template developed and approved by Legal and Compliance
- Customer service team trained on explanation delivery
- Complaints related to unexplained credit refusals monitored as a KPI

**Implementation Steps:**

| Step | Action | Owner | Due |
|---|---|---|---|
| 1 | ML Engineering implements SHAP layer on NP-001 output pipeline | ML Engineering | Month 1 |
| 2 | Test SHAP outputs for accuracy and stability across sample decisions | ML Engineering | Month 2 |
| 3 | Design customer-facing explanation format - top 3 factors in plain language | Head of Credit Risk | Month 2 |
| 4 | Legal review of customer communication template | General Counsel | Month 2 |
| 5 | Train customer service team on explanation delivery | Head of Customer Operations | Month 3 |
| 6 | Go-live: SHAP explanations integrated into refusal communications | Head of Credit Risk | Month 3 |
| 7 | Monitor complaint rate for unexplained refusals - monthly KPI | AGPO | Ongoing |

---

### CTRL-003 — Governance Review Schedule Formalisation for NP-001

| Field | Detail |
|---|---|
| **Control ID** | CTRL-003 |
| **Source Gap** | Phase 2 - GAP-01: Review schedule not formalised in governance calendar (PARTIAL) |
| **System** | NP-001 Credit Scoring Engine |
| **Regulatory Reference** | EU AI Act Article 9(1) - risk management system maintained on ongoing basis |
| **Control Description** | Add NP-001 Article 9 risk management reviews to the AI Governance Committee calendar on a 6-monthly cycle. AGPO responsible for preparing review materials; Head of Credit Risk sign-off required. |
| **Owner** | Chief Risk Officer |
| **Target Completion** | Q2 2025 |
| **Estimated Cost** | Internal resource only |
| **Status** | ✅ Complete |

**Success Criteria:**
- 6-monthly review dates confirmed in committee calendar for the next 24 months
- Review preparation responsibilities assigned to AGPO
- First review completed on schedule

---

### CTRL-004 — Monitoring to Risk Register Feedback Loop for NP-001

| Field | Detail |
|---|---|
| **Control ID** | CTRL-004 |
| **Source Gap** | Phase 2 - GAP-02: No feedback loop from monitoring to risk register (PARTIAL) |
| **System** | NP-001 Credit Scoring Engine |
| **Regulatory Reference** | EU AI Act Article 9(2)(c) - risk evaluation based on post-market monitoring data |
| **Control Description** | Establish a formal process linking NP-001 performance monitoring data to the Phase 2 risk register. Define specific monitoring thresholds that trigger a mandatory risk register review when breached. |
| **Owner** | Head of Credit Risk |
| **Target Completion** | Q3 2025 |
| **Estimated Cost** | Internal resource only |
| **Status** | 🔴 Not Started |

**Success Criteria:**
- Monitoring thresholds defined for each risk in the NP-001 risk register
- Automated alerting configured to notify the AGPO when thresholds are breached
- Process documented: threshold breach → AGPO notification → risk register review → committee escalation if required
- First threshold breach handled through the new process

**Trigger Thresholds:**

| Risk | Monitoring Metric | Trigger Threshold |
|---|---|---|
| RISK-NP001-01 (Demographic bias) | Approval rate differential across protected groups | > 5% differential triggers review |
| RISK-NP001-04 (Model drift) | Population Stability Index | PSI > 0.2 triggers review |
| RISK-NP001-05 (Data quality) | Missing field rate in input pipeline | > 2% triggers review |

---

### CTRL-005 — Fairness Metrics Definition for NP-001

| Field | Detail |
|---|---|
| **Control ID** | CTRL-005 |
| **Source Gap** | Phase 2 - GAP-06: Fairness metrics not defined (PARTIAL) |
| **System** | NP-001 Credit Scoring Engine |
| **Regulatory Reference** | EU AI Act Article 9(5) - testing against preliminarily defined metrics |
| **Control Description** | Define quantitative fairness metrics and acceptable thresholds for NP-001 - specifically demographic parity ratio and equalised odds difference across all protected characteristic groups. |
| **Owner** | Head of Credit Risk |
| **Target Completion** | Q2 2025 |
| **Estimated Cost** | Internal resource only |
| **Status** | 🟡 In Progress |

**Success Criteria:**
- Fairness metrics formally defined and documented in the NP-001 technical file
- Thresholds approved by the AI Governance Committee
- Metrics integrated into the monthly monitoring dashboard
- Baseline measurement completed against current model

**Proposed Metrics and Thresholds:**

| Metric | Definition | Acceptable Threshold |
|---|---|---|
| Demographic Parity Ratio | Approval rate for protected group / approval rate for reference group | ≥ 0.80 (i.e. no group approved at less than 80% the rate of the highest-approved group) |
| Equalised Odds - TPR | True positive rate parity across groups | < 5% differential |
| Equalised Odds - FPR | False positive rate parity across groups | < 5% differential |

---

### CTRL-006 — Robustness Testing Schedule for NP-002

| Field | Detail |
|---|---|
| **Control ID** | CTRL-006 |
| **Source Gap** | Phase 2 - GAP-05: Robustness testing schedule not formalised (PARTIAL) |
| **System** | NP-002 Fraud Detection System |
| **Regulatory Reference** | EU AI Act Article 15 - accuracy, robustness and cybersecurity |
| **Control Description** | Define and document a formal robustness testing schedule for NP-002, including pass/fail criteria, testing methodology and escalation process if tests fail. |
| **Owner** | Head of Financial Crime |
| **Target Completion** | Q2 2025 |
| **Estimated Cost** | Internal resource only |
| **Status** | 🟡 In Progress |

**Success Criteria:**
- Quarterly robustness testing schedule confirmed in calendar
- Testing methodology documented with pass/fail criteria
- First scheduled test completed and results reported to the AI Governance Committee

**Robustness Testing Scope:**

| Test Type | Frequency | Pass Criterion |
|---|---|---|
| Adversarial transaction injection | Quarterly | Detection rate for adversarial samples ≥ 85% |
| High-volume stress test | Quarterly | No degradation in detection rate at 3x peak transaction volume |
| False positive rate test | Monthly | False positive rate < 0.5% of legitimate transactions |
| Model drift assessment | Monthly | PSI < 0.2; no significant change in feature importance rankings |

---

### CTRL-007 — False Positive SLA for NP-002

| Field | Detail |
|---|---|
| **Control ID** | CTRL-007 |
| **Source Gap** | Phase 2 - GAP (RISK-NP002-01): False positive rate lacks SLA (PARTIAL) |
| **System** | NP-002 Fraud Detection System |
| **Regulatory Reference** | FCA Consumer Duty - avoid foreseeable harm; EU AI Act Article 9 |
| **Control Description** | Define and operationalise a false positive rate SLA for NP-002. Implement automated monitoring against the SLA with monthly reporting to the AI Governance Committee and a customer dispute resolution pathway. |
| **Owner** | Head of Financial Crime |
| **Target Completion** | Q2 2025 |
| **Estimated Cost** | £5,000 - £10,000 |
| **Status** | ✅ Complete |

**Success Criteria:**
- SLA defined: < 0.5% of legitimate transactions incorrectly blocked
- Automated monitoring live and reporting against SLA monthly
- Customer dispute resolution pathway operational with 24-hour resolution target
- Monthly false positive rate report added to AI Governance Committee agenda

---

## Summary Dashboard

| Control | System | Gap Severity | Owner | Target | Status |
|---|---|---|---|---|---|
| CTRL-001 Bias audit | NP-001 | 🔴 Non-Compliant | Head of Credit Risk | Q2 2025 | 🟡 In Progress |
| CTRL-002 Explainability layer | NP-001 | 🔴 Non-Compliant | Head of Credit Risk | Q2 2025 | 🟡 In Progress |
| CTRL-003 Review schedule | NP-001 | 🟡 Partial | CRO | Q2 2025 | ✅ Complete |
| CTRL-004 Monitoring feedback loop | NP-001 | 🟡 Partial | Head of Credit Risk | Q3 2025 | 🔴 Not Started |
| CTRL-005 Fairness metrics | NP-001 | 🟡 Partial | Head of Credit Risk | Q2 2025 | 🟡 In Progress |
| CTRL-006 Robustness testing | NP-002 | 🟡 Partial | Head of Financial Crime | Q2 2025 | 🟡 In Progress |
| CTRL-007 False positive SLA | NP-002 | 🟡 Partial | Head of Financial Crime | Q2 2025 | ✅ Complete |

**Overall status:** 2 of 7 controls complete · 4 in progress · 1 not started

---

## Escalation and Reporting

- Controls tracker reviewed monthly by AGPO
- Status reported quarterly to AI Governance Committee
- Any control that misses its target date is escalated to the CRO with a revised timeline and documented rationale
- Full closure of all seven controls is a prerequisite for Phase 4 (AI Audit and Compliance Monitoring) to commence

---

*NorthPoint Financial Services · AI Governance Office*
*Questions: ai-governance@northpoint-financial.example*
