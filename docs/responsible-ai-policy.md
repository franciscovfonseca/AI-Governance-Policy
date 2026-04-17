# Responsible AI Policy — NorthPoint Financial Services
**Document Type:** Corporate Policy
**Classification:** Internal — All Staff
**Version:** 1.0
**Effective Date:** Q2 2025
**Policy Owner:** Chief Risk Officer
**Review Cycle:** Annual
**Status:** ✅ Approved — AI Governance Committee

---

## 1. Purpose and Scope

This policy establishes NorthPoint Financial Services' commitments for the responsible development, procurement, deployment and ongoing operation of artificial intelligence systems across the organisation.

It applies to:
- All AI systems developed internally by NorthPoint
- All AI systems procured from third-party vendors and deployed by NorthPoint
- All employees, contractors and third parties involved in the design, deployment or operation of AI systems on NorthPoint's behalf

This policy does not distinguish between AI systems based on the technology used. Any system that uses machine learning, automated decision-making or generative AI to produce outputs that affect customers, employees or business operations is in scope.

---

## 2. Context and Rationale

NorthPoint operates in a regulated environment where AI systems are increasingly making or materially influencing consequential decisions - including whether customers are offered credit, whether transactions are flagged as fraudulent and how customers receive support.

The EU AI Act (Regulation 2024/1689), which applies to NorthPoint as a deployer of AI systems in the EU market, creates legally binding obligations for systems classified as HIGH RISK. Two of NorthPoint's four production AI systems carry this classification. Non-compliance carries enforcement risk including fines of up to €30 million or 6% of global annual turnover.

Beyond regulatory compliance, responsible AI governance is a business imperative. AI systems that produce biased, opaque or unreliable outputs create customer harm, regulatory exposure and reputational damage. This policy exists to prevent those outcomes.

---

## 3. Foundational Principles

NorthPoint's approach to responsible AI is grounded in five principles. Each principle is paired with the operational process that enforces it - because principles without process are decoration.

---

### Principle 1: Fairness

**Commitment:** NorthPoint's AI systems will not produce outcomes that unlawfully discriminate against individuals on the basis of protected characteristics including race, ethnicity, gender, age and disability.

**What this means in practice:**
- Every AI system that makes or materially influences decisions affecting individuals must undergo a bias and fairness assessment before deployment
- HIGH RISK systems must demonstrate demographic parity and equalised odds across all relevant protected characteristic groups
- Bias monitoring is conducted quarterly for HIGH RISK systems and annually for LIMITED RISK systems
- Proxy variables that correlate with protected characteristics must be identified and assessed before being used as model inputs

**Regulatory grounding:** EU AI Act Article 10 (data governance and bias obligations); UK Equality Act 2010; FCA Consumer Duty

---

### Principle 2: Transparency

**Commitment:** NorthPoint's customers and employees will be informed when AI systems play a material role in decisions that affect them.

**What this means in practice:**
- Customers must be informed at the start of any AI-assisted interaction (EU AI Act Article 50 - conversational AI)
- Customers who receive a consequential automated decision - such as a credit refusal or a transaction hold - are entitled to a meaningful explanation of the factors that drove that decision
- Internally deployed AI systems used in HR or performance management decisions must be disclosed to affected employees
- Marketing and personalisation AI systems are subject to transparency obligations under GDPR Article 13/14

**Regulatory grounding:** EU AI Act Articles 13 and 50; GDPR Articles 13, 14 and 22; FCA Consumer Duty

---

### Principle 3: Accountability

**Commitment:** Every AI system operated by NorthPoint has a named, senior owner who is personally accountable for its governance, performance and compliance.

**What this means in practice:**
- System ownership is a mandatory field in the AI inventory - no system may be registered without a named owner at Head of Function level or above
- System Owners are responsible for ensuring their systems comply with this policy and all applicable regulatory obligations
- System Owners are notified within 24 hours of any incident involving their system
- Ownership transfers must be formally documented and approved by the AI Governance Programme Office

**Current system ownership:**

| System | Owner |
|---|---|
| NP-001 Credit Scoring Engine | Head of Credit Risk |
| NP-002 Fraud Detection System | Head of Financial Crime |
| NP-003 Customer Support Chatbot | Head of Customer Operations |
| NP-004 Marketing Personalisation AI | Head of Marketing |

**Regulatory grounding:** EU AI Act Article 9 (risk management system ownership); NIST AI RMF - GOVERN function

---

### Principle 4: Safety and Robustness

**Commitment:** NorthPoint's AI systems are tested for safety and reliability before deployment and monitored continuously throughout their operational lifetime.

**What this means in practice:**
- All AI systems undergo performance testing against defined benchmarks before deployment
- HIGH RISK systems undergo adversarial testing - including red-teaming and stress testing under edge-case conditions - before deployment and after every material model update
- Model performance is monitored continuously; drift thresholds are defined and trigger mandatory review when breached
- HIGH RISK systems maintain a formal retraining schedule documented in the AI inventory
- Robustness testing for systems making real-time automated decisions (including NP-002) is conducted quarterly with results reported to the AI Governance Committee

**Regulatory grounding:** EU AI Act Article 15 (accuracy, robustness and cybersecurity); NIST AI RMF - MEASURE function

---

### Principle 5: Human Oversight

**Commitment:** Consequential decisions made or materially influenced by AI systems are subject to meaningful human review. Rubber-stamp approvals are explicitly prohibited.

**What this means in practice:**
- "Meaningful" human review means the reviewer has sufficient information, time and authority to override the AI recommendation - not simply confirm it
- All HIGH RISK automated decisions must have a documented human oversight mechanism registered in the AI inventory
- Human reviewers must document their rationale when overriding an AI recommendation
- Override rates are monitored as a governance metric - sustained low override rates in HIGH RISK systems trigger a review of whether human oversight is genuinely meaningful
- Staff operating AI-assisted decision systems receive mandatory training on the limits of AI reliability and their authority to override

**Regulatory grounding:** EU AI Act Article 14 (human oversight); NIST AI RMF - GOVERN function; FCA Consumer Duty

---

## 4. AI Lifecycle Obligations

This policy applies across the full AI lifecycle. The obligations at each stage are:

| Lifecycle Stage | Obligation |
|---|---|
| **Ideation and Design** | Document intended use case, affected stakeholders and preliminary risk classification before development begins |
| **Procurement** | Vendor contracts must include equivalent governance obligations; vendor systems are subject to the same review process as internally built systems |
| **Pre-deployment Review** | All systems must complete the AI Use Case Review Process and receive formal approval before deployment |
| **Registration** | Approved systems are registered in the AI System Inventory with all mandatory fields completed |
| **Operation** | System Owners are responsible for ongoing monitoring, incident reporting and compliance with review schedules |
| **Material Change** | Any material change to a system's purpose, model, data inputs or deployment scope triggers a new use case review |
| **Decommission** | Systems removed from operation are formally deregistered; data retention obligations are fulfilled; decommission is documented in the inventory |

---

## 5. Third-Party and Vendor AI

AI systems developed by third parties and deployed by NorthPoint are subject to the same obligations as internally built systems. NorthPoint is the deployer and bears regulatory accountability under the EU AI Act regardless of who built the system.

Vendor contracts for AI systems must include:
- Disclosure of the AI system's purpose, training data sources and known limitations
- Commitment to provide technical documentation sufficient for NorthPoint to meet its Article 11 obligations
- Notification requirements for material model updates or changes
- Cooperation with NorthPoint audits and regulatory enquiries
- Data processing agreements covering any personal data used by the system

---

## 6. Incident Response

Any incident involving an AI system - including unexpected outputs, customer harm, data breach or regulatory enquiry - must be reported to the AI Governance Programme Office within 24 hours of discovery.

The AGPO will triage the incident and escalate to the AI Governance Committee if the incident is material. Material incidents include:
- Customer harm caused by an AI decision
- Evidence of discriminatory outcomes
- Regulatory contact or formal enquiry
- System compromise or adversarial manipulation
- Model failure affecting more than 1% of transactions in a 24-hour period

System Owners retain immediate suspension authority - they may suspend an AI system without committee approval if they believe it presents an immediate risk to customers or the organisation.

---

## 7. Training and Awareness

All employees who interact with, operate or make decisions based on AI system outputs must complete mandatory AI literacy training covering:
- NorthPoint's AI principles and this policy
- How to identify and report AI-related incidents
- Their authority and obligation to override AI recommendations when appropriate
- The limits of AI reliability and the importance of human judgement

Training is completed at onboarding and refreshed annually. Completion rates are reported quarterly to the AI Governance Committee.

---

## 8. Policy Governance

| Field | Detail |
|---|---|
| **Policy Owner** | Chief Risk Officer |
| **Maintained by** | AI Governance Programme Office |
| **Approved by** | AI Governance Committee |
| **Review cycle** | Annual - or triggered by material regulatory change |
| **Next review** | Q2 2026 |
| **Exceptions** | Exceptions require written approval from the Chief Risk Officer with documented rationale |

---

*NorthPoint Financial Services · AI Governance Office*
*Questions: ai-governance@northpoint-financial.example*
