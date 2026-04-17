# AI Use Case Review and Approval Process — NorthPoint Financial Services
**Document Type:** Process Documentation
**Classification:** Internal — All Staff
**Version:** 1.0
**Effective Date:** Q2 2025
**Owner:** AI Governance Programme Office
**Status:** ✅ Approved — AI Governance Committee

---

## Purpose

This document defines the process by which new AI use cases are submitted, reviewed and approved at NorthPoint Financial Services. No AI system may be deployed into a production environment without completing this process and receiving formal approval.

The process is risk-proportionate. Lower-risk systems move quickly through a two-week Standard Review. Higher-risk systems receive the rigorous scrutiny their risk level demands - a four-to-six-week Enhanced Review with cross-functional involvement and committee-level approval.

The principle is simple: simpler use cases should not be burdened by heavyweight governance. Consequential use cases should not be rushed through lightweight governance.

---

## Scope

This process applies to:
- New AI systems being built internally
- AI systems being procured from third-party vendors
- Existing AI systems undergoing a material change in purpose, model, data inputs or deployment scope
- Proof-of-concept or pilot deployments that interact with real customer or employee data

This process does not apply to:
- Research and development activities using entirely synthetic data
- Academic or training exercises with no production deployment intent

If in doubt, contact the AI Governance Programme Office at ai-governance@northpoint-financial.example before proceeding.

---

## Process Overview

The review process has six stages:

```
Stage 1: Submission
Stage 2: Intake Triage
Stage 3: Review (Standard or Enhanced)
Stage 4: Approval Decision
Stage 5: Registration and Deployment
Stage 6: Ongoing Monitoring
```

Material changes to a deployed system restart the process from Stage 1.

---

## Stage 1 — Submission

**Who submits:** The System Owner - or a nominated representative at Head of Function level or above.

**How to submit:** Complete the AI Use Case Submission Form and send to ai-governance@northpoint-financial.example. The form is available from the AI Governance Programme Office.

**What the form captures:**

| Section | Required Information |
|---|---|
| System description | What the system does, intended users and affected populations |
| Business justification | Why this system is needed and what problem it solves |
| Data inputs | What data the system uses, including personal data categories |
| Decision type | Whether the system makes automated decisions or provides recommendations |
| Deployment scope | Which business units, geographies and customer segments are affected |
| Proposed System Owner | Named individual at Head of Function level or above |
| Vendor information | If third-party - vendor name, system documentation and contract status |

**Acknowledgement:** The AGPO acknowledges receipt within two business days and assigns a use case reference number.

---

## Stage 2 — Intake Triage

**Performed by:** AI Governance Programme Office

**Timeline:** Within three business days of submission

**Triage outcomes:**

| Outcome | Criteria | Next Step |
|---|---|---|
| **Prohibited** | Use case falls within EU AI Act Annex I prohibited practices (e.g. social scoring, real-time biometric surveillance in public spaces, subliminal manipulation) | Immediate rejection - CRO notified within 24 hours - submitter informed with written explanation |
| **Standard Review** | MINIMAL or LIMITED RISK classification | Proceed to Standard Review |
| **Enhanced Review** | HIGH RISK classification under EU AI Act Annex III | Proceed to Enhanced Review |
| **Clarification Required** | Insufficient information to classify | AGPO contacts submitter within three business days - clock pauses until response received |

**Risk classification:** The AGPO applies the EU AI Act four-tier risk framework to classify the submission. Where classification is unclear the AGPO consults Legal and the DPO before finalising.

---

## Stage 3a — Standard Review (MINIMAL and LIMITED RISK)

**Timeline:** 2 weeks from triage completion

**Conducted by:** AI Governance Programme Office

**Review checklist:**

| Check | Description |
|---|---|
| Classification confirmed | Risk tier is correct and documented with reasoning |
| Data lawfulness | Legal basis for personal data processing confirmed with DPO |
| Disclosure mechanism | If LIMITED RISK - AI disclosure to users is designed and documented |
| System Owner confirmed | Named owner at appropriate seniority has accepted accountability |
| Inventory entry prepared | Draft inventory entry completed with all mandatory fields |
| Monitoring plan | Minimum monitoring requirements defined for the system's risk tier |

**Outcome:** AGPO issues approval or rejection in writing within the two-week window. If rejected the submitter receives written reasons and may resubmit after addressing the identified gaps.

---

## Stage 3b — Enhanced Review (HIGH RISK)

**Timeline:** 4-6 weeks from triage completion

**Conducted by:** AGPO with cross-functional review panel

**Review panel composition:**

| Function | Role in Review |
|---|---|
| AI Governance Programme Office | Process lead - coordinates review, prepares committee paper |
| Legal | Regulatory obligation mapping; contract review for vendor systems |
| Data Protection Officer | DPIA; data governance obligations under Article 10 |
| Information Security | Security assessment; adversarial testing requirements |
| ML Engineering | Technical documentation review; performance benchmark validation |
| Business Risk | Business risk assessment; impact on existing risk appetite |

**Review requirements:**

| Requirement | Description |
|---|---|
| Structured risk assessment | Full risk register using Phase 2 methodology - likelihood, impact, mitigations and residual risk |
| Technical documentation | System architecture, training data description, performance benchmarks and known limitations |
| Bias and fairness evaluation | Assessment across all relevant protected characteristics; proxy variable review |
| Human oversight design | Documented oversight mechanism meeting Article 14 requirements |
| Monitoring plan | Performance metrics, drift thresholds, review schedule and escalation triggers |
| EU AI Act compliance checklist | Article 9-15 obligations mapped and compliance status confirmed |
| Post-market monitoring plan | How the system will be monitored after deployment per Article 9(7) |

**Committee paper:** The AGPO prepares a structured committee paper summarising review findings, open issues and a recommendation for the AI Governance Committee. The paper is circulated to committee members five business days before the scheduled meeting.

---

## Stage 4 — Approval Decision

**Standard Review:** AGPO issues written approval or rejection. No committee meeting required.

**Enhanced Review:** AI Governance Committee reviews the AGPO paper and votes at the next scheduled quarterly meeting. Where the timeline does not permit waiting for the next quarterly meeting an extraordinary session may be convened by the CRO.

**Possible outcomes:**

| Decision | Meaning | Next Step |
|---|---|---|
| **Approved** | System meets all requirements and may proceed to deployment | AGPO issues approval letter; system registered in inventory |
| **Approved with Conditions** | System may proceed subject to specific conditions being met before go-live | AGPO issues conditional approval; conditions tracked to closure |
| **Deferred** | Decision requires additional information or remediation | AGPO issues deferral notice with specific requirements; review restarts from Stage 3 when requirements are met |
| **Rejected** | System does not meet requirements and cannot be approved in its current form | AGPO issues rejection with written reasons; submitter may appeal to CRO within 20 business days |

---

## Stage 5 — Registration and Deployment

**Following approval:**

1. System Owner confirms deployment readiness in writing to the AGPO
2. AGPO completes the AI System Inventory entry with all mandatory fields and supporting documentation
3. AGPO issues a system registration certificate with the assigned system ID (format: NP-###)
4. System Owner confirms go-live date to AGPO
5. AGPO schedules the first governance review in the AI Governance Committee calendar

**Deployment checklist (System Owner responsibility):**

- [ ] All approval conditions confirmed as met
- [ ] System documentation uploaded to inventory
- [ ] Monitoring dashboards live and alerting configured
- [ ] Human oversight process briefed to operational staff
- [ ] Customer disclosure mechanisms live (if required)
- [ ] Incident reporting process confirmed with operational team

---

## Stage 6 — Ongoing Monitoring and Review

Deployment is not the end of governance - it is the beginning of ongoing accountability.

**Review schedules by risk tier:**

| Risk Tier | Review Frequency | Reviewer | Escalation |
|---|---|---|---|
| HIGH RISK | Every 6 months (or quarterly for systems with open compliance gaps) | System Owner - findings reviewed by AGPO | Material findings escalated to AI Governance Committee |
| LIMITED RISK | Annually | System Owner - findings reviewed by AGPO | Material findings escalated to AGPO |
| MINIMAL RISK | Annually | System Owner | Self-certification submitted to AGPO |

**Material change triggers:** The following changes require a new use case submission regardless of the system's review schedule:
- Change in the system's primary purpose or intended use
- Significant update to the underlying model (retraining on substantially different data)
- Expansion of deployment scope to new geographies, customer segments or business units
- Integration with a new data source containing personal data
- Change in the automated decision threshold affecting a material number of customers

---

## Process Timeline Summary

| Stage | Timeline | Responsibility |
|---|---|---|
| Submission acknowledgement | 2 business days | AGPO |
| Intake triage | 3 business days | AGPO |
| Standard Review decision | 2 weeks from triage | AGPO |
| Enhanced Review - panel review | 3-4 weeks from triage | Review panel |
| Enhanced Review - committee decision | 4-6 weeks from triage | AI Governance Committee |
| Registration following approval | 5 business days | AGPO |

---

## Contacts

| Query | Contact |
|---|---|
| Submission form and process questions | ai-governance@northpoint-financial.example |
| Classification questions | AGPO or your Functional AI Champion |
| Urgent incidents | CRO via direct line; AGPO within 24 hours |

---

*NorthPoint Financial Services · AI Governance Office*
*Questions: ai-governance@northpoint-financial.example*
