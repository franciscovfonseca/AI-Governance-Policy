# AI Governance Operating Model — NorthPoint Financial Services
**Document Type:** Governance Framework
**Classification:** Internal — Restricted
**Version:** 1.0
**Effective Date:** Q2 2025
**Owner:** Chief Risk Officer
**Status:** ✅ Approved — Board Risk and Audit Committee

---

## Purpose

This document defines NorthPoint Financial Services' AI Governance Operating Model - the organisational structure, roles, decision authority and integration points that make AI governance operational rather than aspirational.

A governance policy defines what NorthPoint is committed to. This operating model defines who is responsible for delivering it, how decisions get made and where accountability sits at every level of the organisation.

---

## Governance Structure Overview

NorthPoint's AI governance operates across five tiers. Each tier has defined responsibilities and a clear escalation path to the tier above.

```
Board Risk and Audit Committee
        ↓
  Chief Risk Officer
        ↓
AI Governance Committee
        ↓
AI Governance Programme Office
        ↓
Functional AI Champions (x8)
        ↓
    System Owners
```

---

## Tier 1 — Board Risk and Audit Committee

**Role:** Strategic oversight and ultimate accountability for AI governance

**Responsibilities:**
- Reviews the AI governance programme annually against strategy and regulatory developments
- Approves HIGH RISK system deployments escalated by the AI Governance Committee where board-level sign-off is required
- Oversees material AI incidents and receives post-incident reports
- Approves the AI governance budget and resource allocation
- Receives annual AI governance dashboard covering portfolio risk profile, compliance status and incident summary

**Meeting frequency:** Annual AI governance review; ad hoc for escalated HIGH RISK approvals and material incidents

**Key metric reviewed:** Portfolio-level EU AI Act compliance status; number of open HIGH RISK compliance gaps; material incidents in the period

---

## Tier 2 — Chief Risk Officer

**Role:** Executive sponsor and policy owner

**Responsibilities:**
- Owns the Responsible AI Policy and is accountable for its implementation
- Chairs the AI Governance Committee
- Serves as final escalation authority for contested governance decisions
- Represents AI governance at board level
- Approves policy exceptions with documented rationale

**Delegated authority:** May approve HIGH RISK system deployments without full committee meeting in time-sensitive situations - with retrospective committee ratification required within 30 days

---

## Tier 3 — AI Governance Committee

**Role:** Primary decision-making body for AI governance across NorthPoint

**Composition:**

| Role | Member | Voting |
|---|---|---|
| Chair | Chief Risk Officer | Yes |
| Technology | Chief Technology Officer | Yes |
| Data and Privacy | Data Protection Officer | Yes |
| Legal | General Counsel | Yes |
| Security | Chief Information Security Officer | Yes |
| Finance | Chief Financial Officer | Observer |

**Responsibilities:**
- Approves all HIGH RISK system deployments submitted through the use case review process
- Reviews and approves updates to the Responsible AI Policy and this operating model
- Reviews quarterly AI governance dashboard - portfolio compliance status, open gaps and incident summary
- Escalates material issues to the Board Risk and Audit Committee
- Reviews and approves the annual AI governance training programme

**Meeting frequency:** Quarterly scheduled; extraordinary meetings convened for material incidents or time-sensitive HIGH RISK approvals

**Quorum:** Chair plus three voting members

**Decision record:** All committee decisions are minuted and stored by the AI Governance Programme Office for audit purposes

---

## Tier 4 — AI Governance Programme Office

**Role:** Operational backbone of the AI governance programme

**Staffing:** 1.5 FTE initially - AI Governance Manager (1.0 FTE) and AI Governance Analyst (0.5 FTE)

**Responsibilities:**

*Inventory and registry:*
- Maintains the AI System Inventory as the authoritative record of all AI systems in the portfolio
- Processes system registrations, updates and decommissions
- Flags inventory gaps and escalates to System Owners

*Use case review:*
- Receives all new AI use case submissions
- Conducts intake triage to determine review pathway
- Manages Standard Reviews end-to-end (approves MINIMAL and LIMITED RISK systems)
- Coordinates Enhanced Reviews - assembles review panels, manages timeline and prepares committee papers for HIGH RISK approvals

*Compliance monitoring:*
- Tracks open compliance gaps from Phase 2 risk assessments and subsequent reviews
- Produces quarterly compliance dashboard for the AI Governance Committee
- Manages the controls implementation plan and chases owners on overdue actions

*Training and awareness:*
- Designs and delivers the mandatory AI literacy training programme
- Tracks completion rates and reports to the committee quarterly

*Incident coordination:*
- Receives all AI incident reports within the 24-hour window
- Triages incidents and escalates material incidents to the CRO and committee
- Coordinates post-incident reviews and ensures lessons learned are captured

---

## Tier 5a — Functional AI Champions

**Role:** Embedded governance contacts within each business unit

**Coverage:** Eight business units - Credit, Financial Crime, Customer Operations, Marketing, Technology, Risk, Legal and Compliance, and HR

**Responsibilities:**
- Serve as the first point of contact for colleagues with AI governance questions
- Help business unit teams complete use case submission forms
- Escalate potential AI uses that may not have been formally submitted to the AGPO
- Communicate policy updates and training requirements to their business unit
- Attend quarterly AI Champions Forum to share learnings and raise emerging issues

**Time commitment:** Approximately 10-15% of working time. Champions are typically senior managers within their function.

**Appointment:** Nominated by business unit heads and approved by the AGPO. Term: 2 years, renewable.

---

## Tier 5b — System Owners

**Role:** Day-to-day accountability for individual AI system compliance

**Current System Owners:**

| System | Owner | Review Frequency |
|---|---|---|
| NP-001 Credit Scoring Engine | Head of Credit Risk | 6-monthly |
| NP-002 Fraud Detection System | Head of Financial Crime | Quarterly |
| NP-003 Customer Support Chatbot | Head of Customer Operations | Annual |
| NP-004 Marketing Personalisation AI | Head of Marketing | Annual |

**Responsibilities:**
- Ensure their system operates in compliance with the Responsible AI Policy and all applicable regulatory obligations at all times
- Maintain the system's entry in the AI inventory - keeping technical documentation, risk assessments and monitoring data current
- Report incidents to the AGPO within 24 hours of discovery
- Complete scheduled governance reviews on time and submit findings to the AGPO
- Approve or reject material changes to their system - and submit a new use case review if the change triggers re-assessment
- Immediate suspension authority: System Owners may suspend their system without committee approval if it presents an immediate risk

---

## Decision Authority Matrix

| Decision | System Owner | AGPO | AI Governance Committee | CRO | Board |
|---|---|---|---|---|---|
| Register MINIMAL RISK system | Submits | Approves | - | - | - |
| Register LIMITED RISK system | Submits | Approves | - | - | - |
| Register HIGH RISK system | Submits | Coordinates | **Approves** | - | - |
| Register HIGH RISK system (board escalation) | Submits | Coordinates | Reviews | **Approves** | Ratifies |
| Suspend a system (incident) | **Immediate authority** | Notified | - | Notified | - |
| Policy exception | Requests | Reviews | - | **Approves** | - |
| Policy update | - | Drafts | **Approves** | Ratifies | - |
| Annual programme review | - | Prepares | Contributes | Presents | **Approves** |

---

## Integration with Existing Functions

The AI Governance Operating Model is designed to work with NorthPoint's existing governance structures rather than duplicate them.

| Function | Integration Point |
|---|---|
| **Enterprise Risk Management** | AI risks are registered in the enterprise risk register; AI Governance Committee reports to the Risk Committee |
| **Data Protection** | DPO sits on the AI Governance Committee; DPIA process is triggered alongside Enhanced Reviews for systems processing personal data |
| **Information Security** | CISO sits on the AI Governance Committee; security assessments are part of Enhanced Review for HIGH RISK systems |
| **Legal and Compliance** | General Counsel sits on the AI Governance Committee; regulatory change monitoring feeds into policy review cycle |
| **Procurement** | Vendor AI systems trigger the use case review process; procurement policy updated to include AI governance obligations in vendor contracts |
| **Internal Audit** | AI governance programme is included in the internal audit schedule; AGPO provides audit support and documentation |

---

## Governance Metrics and Reporting

The AGPO produces the following governance reporting:

| Report | Frequency | Audience | Key Metrics |
|---|---|---|---|
| AI Governance Dashboard | Quarterly | AI Governance Committee | Portfolio compliance status, open gaps, review queue, incident count |
| System Owner Compliance Summary | Quarterly | System Owners | Per-system review status, open actions, upcoming review dates |
| Annual Governance Report | Annual | Board Risk and Audit Committee | Programme-level performance, regulatory developments, resource requirements |
| Incident Report | As required | CRO and Committee | Incident description, impact, root cause, remediation actions |

---

*NorthPoint Financial Services · AI Governance Office*
*Questions: ai-governance@northpoint-financial.example*
