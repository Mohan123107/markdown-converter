# TILLI SOFTWARE
# ARTIFICIAL INTELLIGENCE GOVERNANCE POLICY
# AND ARTIFICIAL INTELLIGENCE MANAGEMENT SYSTEM (AIMS)
Volume I — Governance Policy (Master Progressive Build)
Document ID: AIMS-001
Version: 3.5 (Working Master)
Framework Alignment: ISO/IEC 42001:2023 | ISO/IEC 27001:2022

# TABLE OF CONTENTS
# DOCUMENT CONTROL
Organization: Tilli Software
Document ID: AIMS-001 (Consolidated)
Version: 1.0
Adopted By: Board of Directors
Owner: CTO (Operational) / AI Governance Lead (Oversight)
Effective Date: [Insert Date]
Review Cycle: Annual
Applies To: Engineering, Product, Security, Compliance, Data, Operations
Systems Referenced: GitHub, Jira, SharePoint, GitHub Actions, Datadog, AWS


# PART A — AI GOVERNANCE POLICY
## INTRODUCTION
Tilli recognizes that Artificial Intelligence (AI) systems introduce operational, ethical, legal, security, and reputational risks alongside significant innovation opportunities. This Policy establishes the governance framework under which AI systems are designed, developed, deployed, and operated across the organization.
This Policy forms the foundation of Tilli’s Artificial Intelligence Management System (AIMS) and supports alignment with ISO/IEC 42001 principles. It also integrates with the Company’s ISO 27001 Information Security Management System (ISMS).
## ARTICLE I — PURPOSE
(ISO 42001 Clauses 4.1, 4.2, 5.1)
This Artificial Intelligence Governance Policy establishes the Artificial Intelligence Management System (AIMS) of Tilli Software (the “Company”).
Tilli recognizes that Artificial Intelligence (AI) systems introduce operational, ethical, legal, security, regulatory, financial, and reputational risks alongside significant innovation opportunities.
This Policy establishes the governance framework under which AI systems are designed, developed, validated, deployed, monitored, and operated across the organization. It defines accountability structures, risk management requirements, documentation standards, validation controls, monitoring expectations, incident management protocols, and Board oversight mechanisms necessary to ensure responsible and sustainable AI adoption.
The purpose of this Policy is to:
1. Ensure responsible, secure, and compliant deployment of Artificial Intelligence systems;
2. Align Company practices with ISO/IEC 42001:2023;
3. Integrate AI governance within the Company’s ISO 27001 Information Security Management System (ISMS);
4. Mitigate financial, operational, legal, regulatory, and reputational risks;
5. Provide structured oversight by executive leadership and the Board;
6. Establish lifecycle governance from intake through retirement;
7. Define accountability, documentation standards, validation requirements, monitoring controls, and audit mechanisms.
## ARTICLE II — DEFINITIONS
(ISO 42001 Clause 3)
**Artificial Intelligence System (AI System): **
Any software system utilizing machine learning, statistical modeling, algorithmic inference, generative AI, large language models, rule-based AI, or similar techniques to produce predictions, classifications, recommendations, automated decisions, or generated outputs.
**High-Risk AI System: **
An AI system capable of materially affecting financial transactions, fraud detection outcomes, customer eligibility, regulatory compliance, consumer rights, credit decisions, or material operational decisions.
**Moderate-Risk AI System: **
AI systems influencing customer-facing analytics, workflow optimization, productivity augmentation, or operational decision-support without direct regulatory or financial decision authority.
**Low-Risk AI System: **
Internal productivity tools, automation utilities, or limited-scope features with minimal customer or regulatory impact.
**Client AI Restriction: **
A contractual, regulatory, or formally documented client directive prohibiting or limiting the use of Artificial Intelligence systems within a specific tenant, deployment, or environment.
**AI-Restricted Environment: **
A product instance or configuration where AI functionality is disabled pursuant to Client AI Restriction requirements.
## ARTICLE III — SCOPE
(ISO 42001 Clauses 4.3, 4.4)
This Policy applies to all AI-enabled systems developed, integrated, or deployed by the Company across its products and services.
It governs internally developed AI systems (including proprietary AI engines such as Jareis), third-party AI integrations, and any hybrid AI architectures deployed within development, staging, or production environments.
This Policy applies to all teams contributing to AI-powered systems, including:
- Engineering;
- Product Management;
- Security and Information Security;
- Data and Analytics;
- Compliance and Legal;
- Operations and Infrastructure.
Where a Client AI Restriction exists, AI functionality must be disabled for the designated tenant or environment, and enforcement must be technically verifiable, auditable, and continuously monitored.
Products currently in scope include (but are not limited to):
• tilliX
• tilliPay
• Nudge
• Nudge Beacon
• Nudge CPaaS
• tilliArc
• XDEX
• Beacon
• Analytics and integration platforms
• Additional products as designated by leadership
## ARTICLE IV — GOVERNANCE STRUCTURE
(ISO 42001 Clause 5)
The Board establishes the AI Review Committee (ARC) to provide structured oversight of AI risk classification, deployment decisions, validation activities, monitoring controls, incident management, and regulatory alignment.
### Section 4.1 AI Review Committee (ARC)
- AI risk classification and approval authority;
- Approval of High-Risk AI deployments prior to production release;
- Oversight of model validation processes;
- Monitoring oversight and performance review;
- Review and escalation of AI-related incidents;
- Quarterly governance reporting to the Board;
- Oversight of enforcement of AI-Restricted Environments.
### Section 4.2 Roles and Accountability
Clear accountability is required to ensure effective AI governance, risk management, regulatory compliance, and operational integrity across all AI-enabled systems.

| Role | Responsibility |
| --- | --- |
| AI Governance Lead | Oversight of AI risk management, compliance alignment, and policy enforcement. |
| Chief Technology Officer (CTO) | Operational ownership of the Artificial Intelligence Management System. |
| Engineering Lead | Technical implementation, architectural integrity, and enforcement of lifecycle controls. |
| Product Owner | Business justification, lifecycle oversight, and feature approval authority. |
| Security Team | Security review, access control validation, and data protection oversight. |
| Compliance / Legal | Regulatory advisory, contractual review, and legal risk assessment. |

Named individuals and reporting structures: Pending assignment by Executive Leadership.
No AI-enabled feature may be released to production without documented risk ownership and assigned accountability.
## ARTICLE V — GOVERNANCE PRINCIPLES
(ISO 42001 Clauses 5, 6, 8)
All Artificial Intelligence systems developed, integrated, or deployed by the Company shall adhere to clearly defined governance principles designed to ensure responsible, secure, transparent, and risk-aligned implementation.
### 5.1 Responsible AI Use
AI systems must be designed, developed, validated, and operated to minimize harm, prevent misuse, and protect customers, clients, and stakeholders from unintended consequences.
### 5.2 Risk-Based Approach
AI systems shall be assessed and governed proportionate to their potential impact, materiality, and regulatory exposure. Higher-risk systems require enhanced validation, monitoring, and oversight.
### 5.3 Transparency
AI-enabled capabilities should be identifiable where appropriate, and system behavior should be explainable to relevant stakeholders, particularly when influencing financial, eligibility, or customer-impacting decisions.
### 5.4 Human Oversight
AI outputs that influence critical operational, financial, or customer-facing decisions must allow for appropriate human review, override, and escalation mechanisms.
### 5.5 Security and Data Protection
AI systems must comply with the Company’s Information Security Management System (ISMS), including access controls, logging requirements, encryption standards, and secure development practices.
### 5.6 Continuous Improvement
AI systems shall be continuously monitored, evaluated, and improved based on performance trends, risk developments, incident learnings, and regulatory changes.
## ARTICLE VI — AI LIFECYCLE REQUIREMENTS
(ISO 42001 Clause 8.1)
All AI-enabled initiatives must follow a structured lifecycle to ensure consistent governance, documentation, validation, deployment control, and monitoring.
The required lifecycle stages include:
- Business requirement definition;
- Feasibility and impact assessment;
- AI risk assessment and classification;
- Technical design and architecture review;
- Development and secure coding controls;
- Model validation (where applicable);
- Deployment approval;
- Monitoring and observability configuration;
- Periodic review and improvement.
No AI System shall be deployed into production without documented completion of all required lifecycle stages and formal approval where applicable.
## ARTICLE VII — AI RISK MANAGEMENT
(ISO 42001 Clause 6.1)
The Company shall maintain a structured AI Risk Management process aligned with enterprise risk management principles and regulatory expectations.
Each AI-enabled system must maintain an AI Risk Register including:
- Identified risks;
- Risk description;
- Likelihood and impact assessment;
- Mitigation strategy;
- Residual risk evaluation;
- Assigned risk owner;
- Review date and review frequency;
- AI Restriction status (where applicable).
Risk registers must be reviewed prior to production deployment, upon significant changes, and at minimum on a quarterly basis.
## ARTICLE VIII — REQUIRED DOCUMENTATION STANDARDS
(ISO 42001 Clause 7.5)
To ensure audit readiness, traceability, and governance consistency, every AI-enabled system must maintain documented evidence across the lifecycle.
Required documentation includes:
- Business requirements documentation (BRD);
- Functional and technical specifications;
- Architecture diagrams;
- AI risk assessment artifacts;
- Validation reports;
- Deployment approval records;
- Monitoring and observability plans;
- Human oversight mechanisms;
- Feature-to-tenant mapping documentation;
- Data usage and data flow documentation.
Documentation must be version-controlled, accessible to relevant stakeholders, and updated whenever material changes occur.
## ARTICLE IX — MODEL VALIDATION
(ISO 42001 Clause 8.3)
All Moderate-Risk and High-Risk AI Systems shall undergo formal validation prior to production deployment. Model validation ensures conceptual soundness, data integrity, performance reliability, fairness, and ongoing monitoring readiness.
Validation shall include, at minimum:
- Conceptual soundness review of model design and assumptions;
- Training and testing data integrity assessment;
- Reproducibility and consistency testing;
- Performance benchmarking against defined success criteria;
- Bias and fairness testing across relevant populations;
- False positive and false negative analysis (where applicable);
- Stress testing for financial or regulatory impact scenarios;
- Monitoring threshold definition and drift detection criteria.
High-Risk AI Systems require independent validation review prior to production release. Validation artifacts must be documented and retained for audit purposes.
## ARTICLE X — THIRD-PARTY AI GOVERNANCE
(ISO 42001 Clause 8.4; ISO 27001 Annex A.5.19, A.5.20)
When external AI providers or AI-enabled third-party services are utilized, the Company must conduct appropriate vendor due diligence and risk assessment.
Third-party AI governance must include:
- Vendor risk evaluation and security assessment;
- Review of data handling and privacy practices;
- Assessment of contractual obligations and liability terms;
- Confirmation of regulatory compliance alignment;
- Validation that AI-Restricted tenant data is not transmitted to external AI systems;
- Ongoing vendor performance and risk monitoring.
## ARTICLE XI — INCIDENT MANAGEMENT
(ISO 42001 Clause 10; ISO 27001 Annex A.5.24)
AI-related incidents must be managed through a structured incident response process aligned with the Company’s Information Security and operational incident management frameworks.
AI-related incidents include, but are not limited to:
- Material model errors affecting customer outcomes;
- Regulatory compliance breaches;
- Unauthorized AI usage in AI-Restricted environments;
- Security incidents involving AI systems;
- Significant bias or discriminatory outcomes;
- Data leakage related to AI processing.
Incident response actions must include:
1. Logging of incident in the designated tracking system (AI-INCIDENT);
1. Notification of Security and Compliance within 24 hours;
1. Assessment of financial, regulatory, and customer impact;
1. Temporary suspension or disabling of affected feature if required;
1. Root cause analysis documentation;
1. Implementation of corrective and preventive actions;
1. Escalation of material incidents to the ARC and Board where appropriate.
## ARTICLE XII — CHANGE MANAGEMENT
(ISO 42001 Clause 8; ISO 27001 Annex A.8.32)
Changes to AI systems, including model updates, training data changes, prompt modifications, architecture revisions, or expanded deployment scope, must undergo structured change management controls.
Material changes include:
- Introduction of new training datasets;
- Model architecture changes;
- Expansion into new jurisdictions;
- Changes affecting financial or regulatory outcomes;
- Enabling AI functionality for previously AI-Restricted tenants.
Change management requirements include:
1. Triggering the AI-CHANGE workflow;
1. Updated risk assessment and documentation;
1. Re-validation where risk profile changes;
1. ARC approval if risk level is elevated;
1. Formal authorization prior to enabling AI in restricted environments.
## ARTICLE XIII — REPORTING & OVERSIGHT
(ISO 42001 Clause 9.3)
The AI Review Committee (ARC) shall provide structured and periodic reporting to executive leadership and the Board to ensure transparency, accountability, and strategic oversight of AI-related risks and controls.
The Quarterly AI Governance Report shall include:
- Comprehensive AI system inventory;
- Risk classification distribution (Low, Moderate, High);
- Validation status of Moderate and High-Risk systems;
- Summary of AI-related incidents and corrective actions;
- Performance trends and model drift analysis;
- Status of AI-Restricted tenant enforcement;
- Regulatory developments impacting AI governance;
- Governance Key Performance Indicators (KPIs).
Material AI-related incidents, regulatory breaches, or significant risk escalations shall be reported to the Board without delay.
## ARTICLE XIV — DEVELOPER ACKNOWLEDGMENT
(ISO 42001 Clause 7.2)
All personnel contributing to the design, development, validation, deployment, or monitoring of AI systems must annually attest to their understanding of and compliance with this Policy.
Developer acknowledgment shall confirm:
- Compliance with the Artificial Intelligence Management System (AIMS);
- Secure handling of regulated and sensitive data;
- Adherence to AI intake, risk classification, validation, and monitoring requirements;
- Prompt escalation of AI-related incidents;
- Awareness of Client AI Restriction enforcement requirements.
Records of acknowledgment shall be retained for a minimum of five (5) years and be subject to internal audit review.
## ARTICLE XV — INTERNAL AUDIT
(ISO 42001 Clause 9.2)
The Company shall conduct periodic internal audits of the Artificial Intelligence Management System to evaluate effectiveness, compliance, and control integrity.
Internal audit scope shall include:
- Verification of accurate AI risk classification;
- Review of documentation completeness and traceability;
- Validation compliance for Moderate and High-Risk systems;
- Monitoring effectiveness and drift detection adequacy;
- Incident response adequacy and corrective action tracking;
- Verification of AI-Restricted tenant enforcement controls.
Audit findings shall be documented, communicated to executive leadership, and tracked through formal remediation processes.
## ARTICLE XVI — CONTINUAL IMPROVEMENT
(ISO 42001 Clause 10)
The Company is committed to continuous improvement of its Artificial Intelligence Management System.
Continuous improvement activities include:
- Annual review of AI risk posture;
- Policy and procedure updates based on regulatory or operational developments;
- Monitoring effectiveness reassessment;
- Incorporation of audit findings and remediation outcomes;
- Incorporation of stakeholder feedback and emerging best practices.
This Policy shall be reviewed at least annually or upon significant regulatory, technological, or organizational changes.
# BOARD APPROVAL
This Artificial Intelligence Governance Policy is adopted by resolution of the Board of Directors and shall remain in effect until amended or repealed.
Approved on: __________________________
Chairperson: __________________________

# ANNEX A — ISO 42001 & ISO 27001 CROSS-REFERENCE MATRIX
This Annex provides a high-level cross-reference mapping between the Articles of this Artificial Intelligence Governance Policy and relevant clauses of ISO/IEC 42001:2023 and ISO/IEC 27001:2022. This mapping supports audit traceability and standards alignment.

| Policy Article | ISO/IEC 42001 Clause(s) | ISO/IEC 27001 Reference(s) |
| --- | --- | --- |
| Article I — Purpose | 4.1, 4.2, 5.1 | 4.1, 5.1 |
| Article II — Definitions | 3 | — |
| Article III — Scope | 4.3, 4.4 | 4.3 |
| Article IV — Governance Structure | 5 | 5.3, A.5.2 |
| Article V — Governance Principles | 5, 6, 8 | Annex A (General Control Principles) |
| Article VI — AI Lifecycle Requirements | 8.1 | A.8.25, A.8.28 |
| Article VII — AI Risk Management | 6.1 | 6.1.2, A.5.7 |
| Article VIII — Documentation Standards | 7.5 | 7.5, A.5.1 |
| Article IX — Model Validation | 8.3 | A.8.29 |
| Article X — Third-Party AI Governance | 8.4 | A.5.19, A.5.20 |
| Article XI — Incident Management | 10 | A.5.24 |
| Article XII — Change Management | 8 | A.8.32 |
| Article XIII — Reporting & Oversight | 9.3 | 9.3 |
| Article XIV — Developer Acknowledgment | 7.2 | 7.2 |
| Article XV — Internal Audit | 9.2 | 9.2 |
| Article XVI — Continual Improvement | 10 | 10 |

Note: This mapping is indicative and supports governance traceability. Formal certification audits may require expanded control-level mapping to Annex A controls.
