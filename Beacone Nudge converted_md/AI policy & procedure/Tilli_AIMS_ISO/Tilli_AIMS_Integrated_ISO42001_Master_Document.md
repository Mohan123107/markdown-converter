# TILLI SOFTWARE
# ARTIFICIAL INTELLIGENCE MANAGEMENT SYSTEM (AIMS)
## COMPREHENSIVE MASTER DOCUMENT
Includes:
- Volume I — Governance Policy
- Volume II — Procedure Manual
- AIMS-RM-001 — Risk Methodology
- AIMS-OBJ-001 — Objectives & KPIs
- AIMS-TRN-001 — Competency & Training
- AIMS-CTX-001 — Context & Stakeholder Analysis
- AIMS-MR-001 — Management Review
- AIMS-CAPA-001 — Corrective & Preventive Action

# TABLE OF CONTENTS






















































































































# TILLI SOFTWARE
# ARTIFICIAL INTELLIGENCE GOVERNANCE POLICY
# AND ARTIFICIAL INTELLIGENCE MANAGEMENT SYSTEM (AIMS)
Volume I — Governance Policy (Master Progressive Build)
Document ID: AIMS-001
Version: 3.5 (Working Master)
Framework Alignment: ISO/IEC 42001:2023 | ISO/IEC 27001:2022

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
# TILLI SOFTWARE
# ARTIFICIAL INTELLIGENCE GOVERNANCE PROCEDURE MANUAL
Volume II — AI Governance Procedures
Document ID: AIP-PR-001 (Consolidated)
Version: 1.0
Owner: CTO
Applies To: Engineering, Product, Security, Compliance, Data, Operations
Systems Referenced: GitHub, Jira, SharePoint, GitHub Actions, Datadog, AWS

# PART A — PROCEDURAL FRAMEWORK
## 1. PURPOSE
This Procedure Manual operationalizes the Artificial Intelligence Governance Policy (Volume I) and defines the step-by-step lifecycle controls, workflows, approval mechanisms, monitoring requirements, incident response processes, and documentation standards governing all AI-enabled systems.
This Manual ensures consistent execution of the Artificial Intelligence Management System (AIMS) across all applicable teams and environments.
## 2. AI SYSTEM LIFECYCLE WORKFLOW
All AI-enabled initiatives must follow the structured lifecycle defined below. No AI system may bypass any mandatory control stage.
### 2.1 Stage 1 — AI Intake
Trigger: Jira Epic labeled 'AI-INIT'.
Required Intake Information:
- Business objective and justification;
- Product impacted;
- Data classification (PCI, PII, PHI, etc.);
- Tenant impact;
- Jurisdictional exposure;
- Decision impact level (financial, regulatory, operational);
- Client AI Restriction applicability status.
The AI Review Committee (ARC) shall review intake submissions and assign preliminary risk classification.
### 2.2 Stage 2 — Risk Classification
Risk Levels:
- Low — No financial or customer impact;
- Moderate — Customer-facing analytics or workflow optimization;
- High — Financial decisioning, fraud detection, regulatory impact, or customer eligibility outcomes.
High-Risk systems require independent validation prior to production deployment. Risk Classification Form shall be stored in SharePoint.
### 2.3 Stage 3 — Mandatory Documentation
Documentation shall be stored in: /AI Governance/{Product}/{System}/
Required Artifacts:
- Business Requirements Document (BRD);
- Functional Specification;
- Technical Specification;
- Architecture Diagram;
- Risk Classification Form;
- Monitoring Plan;
- Deployment Approval Record;
- Validation Report (where applicable).
Development shall not commence until the documentation folder has been created and initial artifacts uploaded.
### 2.4 Stage 4 — Development Controls
- All AI code must reside in GitHub repositories with protected branches;
- Pull request approval is mandatory prior to merge;
- Model version identifiers must be included in code and logs;
- Secrets must be stored in AWS Secrets Manager;
- Credentials shall never be hardcoded;
- AI invocation logs must be captured in Datadog or equivalent monitoring tool.
Codeowners and branch protection rules shall enforce review discipline.
### 2.5 Stage 5 — Model Validation (Moderate & High Risk)
All Moderate and High-Risk AI systems must undergo formal validation prior to production deployment. Validation ensures conceptual integrity, performance reliability, bias mitigation, regulatory alignment, and operational readiness.
Validation must include:
- Conceptual model design review and documentation of assumptions;
- Training and testing data integrity verification;
- Reproducibility testing to confirm consistent output behavior;
- Performance benchmarking against predefined acceptance criteria;
- Bias and fairness testing across relevant user groups;
- False positive and false negative rate analysis (where applicable);
- Stress testing for financial or regulatory impact scenarios;
- Monitoring thresholds and drift detection configuration definition.
High-Risk AI systems require independent validation review prior to deployment approval. Validation reports must be stored in SharePoint under the designated AI Governance folder.
### 2.6 Stage 6 — Deployment Approval
No AI system may be deployed to production without formal deployment approval.
Deployment approval requires confirmation of:
- Completion of mandatory documentation artifacts;
- Completed risk classification and approval record;
- Completed validation (where required);
- Completed security review;
- Defined rollback plan;
- Verification of AI-Restricted tenant enforcement controls (if applicable).
Production deployment must occur exclusively via approved CI/CD pipelines (GitHub Actions). Manual deployment is prohibited.
### 2.7 Stage 7 — Monitoring & Observability
All AI systems must implement monitoring and observability controls proportionate to their risk classification.
Monitoring controls must include:
- Model version logging;
- Decision metadata logging;
- Performance metric dashboards (Datadog or equivalent);
- Error rate tracking;
- Alert thresholds for abnormal performance;
- Drift monitoring (for predictive models);
- AI-Restricted tenant monitoring to confirm AI remains disabled.
Monitoring Review Cadence:
- High Risk — Quarterly;
- Moderate Risk — Biannual;
- Low Risk — Annual.
### 2.8 Stage 8 — Change Management
All changes to AI systems must follow structured change management procedures. Changes include model updates, prompt revisions, architecture changes, new training datasets, and expansion into new jurisdictions.
Change Management Workflow:
1. Create Jira ticket labeled 'AI-CHANGE';
1. Update risk assessment documentation;
1. Update technical documentation and architecture artifacts;
1. Conduct re-validation if risk profile changes;
1. Obtain ARC approval if risk classification increases;
1. Confirm rollback plan;
1. Document approval record in SharePoint.
### 2.9 Stage 9 — Incident Management
AI-related incidents must be handled through structured response protocols integrated with the Company’s broader incident management framework.
Trigger: Jira ticket labeled 'AI-INCIDENT'.
Mandatory Response Actions:
1. Notify Security and Compliance within 24 hours;
1. Assess financial, operational, and regulatory impact;
1. Disable affected AI feature if required;
1. Conduct root cause analysis;
1. Document corrective and preventive actions;
1. Update AI Risk Register if new risk identified;
1. Escalate material incidents to ARC and Board.
## 3. AI RISK REGISTER PROCEDURE
The AI Risk Register shall be maintained in SharePoint and updated at minimum quarterly.
Required Fields:
- System Name;
- Model Version;
- Risk Level;
- Regulatory Exposure;
- Data Classification;
- Bias Risk;
- Financial Impact;
- Mitigation Controls;
- Monitoring Controls;
- Owner;
- Review Dates;
- AI Restriction Status.
## 4. PROHIBITED USAGE ENFORCEMENT
Violations of AI Policy or Procedure may result in deployment suspension, mandatory security review, disciplinary action, or vendor reassessment.
Unauthorized activation of AI functionality in AI-Restricted environments constitutes a material governance breach.
## 5. QUARTERLY AI GOVERNANCE REPORT PROCEDURE
The AI Review Committee (ARC) shall prepare a Quarterly AI Governance Report to ensure executive and Board-level visibility into AI risk posture, system inventory, performance trends, and regulatory exposure.
The report shall include:
- Comprehensive AI system inventory by product;
- Risk classification distribution summary;
- Validation status of Moderate and High-Risk systems;
- Summary of AI-related incidents and corrective actions;
- Model performance and drift monitoring trends;
- Verification of AI-Restricted tenant enforcement;
- Regulatory or legal developments impacting AI operations;
- Governance KPIs and control effectiveness indicators.
The finalized report shall be stored in SharePoint and presented to executive leadership and the Board.
## 6. DEVELOPER ATTESTATION WORKFLOW
All personnel contributing to AI system development, validation, deployment, or monitoring must complete annual attestation confirming compliance with AIMS requirements.
Attestation process steps:
1. Distribution of annual attestation form;
1. Confirmation of policy review and understanding;
1. Acknowledgment of secure data handling obligations;
1. Affirmation of adherence to intake, validation, and monitoring requirements;
1. Submission of signed acknowledgment to Compliance.
Attestation records shall be retained for a minimum of five (5) years and made available during internal or external audits.
## 7. INTERNAL AUDIT EXECUTION PROCEDURE
The Company shall conduct annual internal audits of the Artificial Intelligence Management System to assess control effectiveness and compliance.
Audit activities shall include:
- Verification of accurate AI risk classification;
- Review of documentation completeness and version control;
- Validation artifact review for Moderate and High-Risk systems;
- Monitoring and drift detection control testing;
- Incident management process review;
- Testing of AI-Restricted tenant enforcement controls.
Audit findings shall be documented in formal audit reports and tracked through remediation workflows until closure.
## 8. AI-RESTRICTED TENANT TECHNICAL ENFORCEMENT PROCEDURE
For clients requiring 'No AI Usage,' the following enforcement controls must be implemented and verified:
- Feature flags disabling AI functionality at tenant level;
- Configuration validation prior to deployment;
- Automated monitoring confirming AI invocation is disabled;
- Logging verification to detect unauthorized AI calls;
- Quarterly verification audit by Engineering and Compliance.
Unauthorized activation of AI functionality in a restricted tenant constitutes a material governance violation and must trigger an AI-INCIDENT workflow.
## 9. RECORD RETENTION & EVIDENCE MANAGEMENT
All AI governance artifacts, validation reports, approval records, risk registers, monitoring dashboards, and attestation forms must be retained in accordance with Company record retention policies.
Minimum retention requirements:
- Validation reports — 5 years;
- Risk Register history — 5 years;
- Incident records — 5 years;
- Developer attestations — 5 years;
- Quarterly Governance Reports — 7 years.
Records must be stored in approved repositories (SharePoint or equivalent) with controlled access and version traceability.

# ANNEX B — PROCEDURE TO ISO CONTROL MAPPING MATRIX
This Annex provides detailed traceability between procedural controls defined in Volume II and relevant ISO/IEC 42001:2023 clauses and ISO/IEC 27001:2022 Annex A controls. It also identifies primary evidence sources and control ownership.

| Procedure Section | ISO 42001 Clause(s) | ISO 27001 Annex A Control(s) | Primary Evidence Source | Control Owner |
| --- | --- | --- | --- | --- |
| 2.1 AI Intake | 8.1 | A.5.2, A.5.7 | Jira (AI-INIT), SharePoint Folder | AI Governance Lead |
| 2.2 Risk Classification | 6.1 | A.5.7 | Risk Classification Form (SharePoint) | AI Governance Lead |
| 2.3 Documentation Controls | 7.5 | A.5.1 | SharePoint Governance Folder | Product Owner |
| 2.4 Development Controls | 8.1 | A.8.25, A.8.28 | GitHub, Codeowners, CI Logs | Engineering Lead |
| 2.5 Model Validation | 8.3 | A.8.29 | Validation Report (SharePoint) | Independent Validator |
| 2.6 Deployment Approval | 8.1 | A.8.32 | Deployment Approval Record, CI Logs | CTO |
| 2.7 Monitoring & Observability | 8.1, 9.1 | A.8.16, A.5.24 | Datadog Dashboards, Logs | Engineering Lead |
| 2.8 Change Management | 8 | A.8.32 | Jira (AI-CHANGE), Updated Risk Assessment | Engineering Lead |
| 2.9 Incident Management | 10 | A.5.24 | Jira (AI-INCIDENT), Incident Report | Security Team |
| 3. AI Risk Register Procedure | 6.1 | A.5.7 | Risk Register (SharePoint) | AI Governance Lead |
| 4. Prohibited Usage Enforcement | 5 | A.5.2 | Incident Logs, Compliance Records | Compliance |
| 5. Quarterly Governance Report | 9.3 | 9.3 | Quarterly Report (SharePoint) | ARC |
| 6. Developer Attestation | 7.2 | 7.2 | Signed Attestation Records | Compliance |
| 7. Internal Audit Execution | 9.2 | 9.2 | Internal Audit Reports | Internal Audit |
| 8. AI-Restricted Enforcement | 8.1 | A.5.2, A.8.16 | Feature Flags, Monitoring Logs | Engineering Lead |
| 9. Record Retention | 7.5 | 7.5 | SharePoint Archive Logs | Compliance |

Note: This mapping supports governance traceability and certification readiness. Expanded control-level mapping may be required for formal ISO certification audits.




# TILLI SOFTWARE
# AI RISK ASSESSMENT METHODOLOGY STANDARD
Document ID: AIMS-RM-001
Version: 1.0
Owner: AI Governance Lead
Approved By: Board of Directors
Effective Date: [Insert Date]
Review Cycle: Annual
Framework Alignment: ISO/IEC 42001:2023 Clause 6.1

## 1. PURPOSE
This Standard defines the formal methodology for identifying, analyzing, evaluating, treating, and monitoring risks associated with Artificial Intelligence (AI) systems deployed by Tilli Software. It establishes a consistent and auditable risk assessment framework aligned with ISO/IEC 42001:2023.
## 2. SCOPE
This methodology applies to all AI-enabled systems across development, staging, and production environments, including internally developed models, third-party AI integrations, and client-specific deployments.
## 3. RISK IDENTIFICATION
Risk identification shall occur during AI intake and be updated during change management and periodic review.
Risk categories include, but are not limited to:
- Model hallucination or inaccurate outputs
- Bias and discriminatory outcomes
- Data leakage or privacy violations
- Prompt injection or adversarial manipulation
- Model drift
- Regulatory non-compliance
- Security vulnerabilities
- Operational disruption
- Unauthorized AI activation in restricted tenants
## 4. LIKELIHOOD SCALE
Likelihood shall be scored using the following scale:

| Score | Description |
| --- | --- |
| 1 | Rare – Highly unlikely to occur |
| 2 | Unlikely – Could occur under limited conditions |
| 3 | Possible – Has occurred in industry or organization |
| 4 | Likely – Expected to occur periodically |
| 5 | Almost Certain – Frequent or recurring occurrence |

## 5. IMPACT SCALE
Impact shall be scored across financial, regulatory, operational, and reputational dimensions.

| Score | Description |
| --- | --- |
| 1 | Negligible – No material impact |
| 2 | Minor – Limited customer or operational effect |
| 3 | Moderate – Customer impact or limited regulatory exposure |
| 4 | Major – Significant financial or regulatory impact |
| 5 | Severe – Material regulatory breach or systemic impact |

## 6. RISK SCORING METHODOLOGY
Risk Score = Likelihood × Impact
Scores shall range from 1 to 25. Risk classification thresholds:

| Score Range | Risk Classification |
| --- | --- |
| 1–6 | Low Risk |
| 7–14 | Moderate Risk |
| 15–25 | High Risk |

## 7. RISK TREATMENT
Risk treatment strategies include:
- Mitigate – Implement control measures to reduce risk
- Transfer – Contractual or insurance-based transfer
- Avoid – Redesign or discontinue AI feature
- Accept – Documented residual risk acceptance
Residual risk for High-Risk AI systems must be formally approved by the AI Review Committee (ARC).
## 8. RISK ACCEPTANCE AUTHORITY
Low Risk – Engineering Lead approval
Moderate Risk – AI Governance Lead approval
High Risk – ARC approval
## 9. RISK REVIEW FREQUENCY
High-Risk AI Systems: Quarterly
Moderate-Risk AI Systems: Biannual
Low-Risk AI Systems: Annual
## 10. DOCUMENTATION & RECORDKEEPING
All risk assessments, scoring worksheets, approval records, and residual risk acceptance documentation shall be stored in SharePoint under the AI Governance repository and retained for a minimum of five (5) years.








# TILLI SOFTWARE
# AI GOVERNANCE OBJECTIVES & KPI FRAMEWORK
Document ID: AIMS-OBJ-001
Version: 1.0
Owner: AI Governance Lead
Approved By: Board of Directors
Effective Date: [Insert Date]
Review Cycle: Annual
Framework Alignment: ISO/IEC 42001:2023 Clause 6.2

## 1. PURPOSE
This document defines measurable Artificial Intelligence (AI) governance objectives and Key Performance Indicators (KPIs) for Tilli Software’s Artificial Intelligence Management System (AIMS). It ensures performance monitoring, accountability, and continual improvement in alignment with ISO/IEC 42001:2023.
## 2. SCOPE
This framework applies to all AI-enabled systems governed under Volume I (Policy) and Volume II (Procedures), including internally developed AI systems and third-party AI integrations.
## 3. AI GOVERNANCE OBJECTIVES
- Ensure all AI systems undergo formal risk classification prior to production deployment.
- Ensure all Moderate and High-Risk AI systems complete documented validation prior to release.
- Prevent unauthorized activation of AI functionality in AI-Restricted tenant environments.
- Ensure timely identification, escalation, and resolution of AI-related incidents.
- Maintain continuous monitoring of AI system performance and drift.
- Ensure compliance with applicable regulatory and contractual AI obligations.
## 4. KEY PERFORMANCE INDICATOR (KPI) MATRIX

| Objective | KPI Metric | Target Threshold | Measurement Frequency | Responsible Owner |
| --- | --- | --- | --- | --- |
| Risk Classification Coverage | % of AI systems risk-classified before production | 100% | Quarterly | AI Governance Lead |
| Validation Compliance | % of Moderate/High-Risk systems independently validated | 100% | Quarterly | Engineering Lead |
| AI-Restricted Enforcement | Unauthorized AI activations in restricted tenants | 0 incidents | Quarterly | Engineering Lead |
| Incident Response Timeliness | % of AI incidents escalated within 24 hours | >= 95% | Quarterly | Security Team |
| Monitoring Coverage | % of AI systems with active monitoring dashboards | 100% | Biannual | Engineering Lead |
| Training Compliance | % of AI contributors completing annual attestation/training | 100% | Annual | Compliance |

## 5. PERFORMANCE MONITORING & REPORTING
KPI performance shall be reviewed during Quarterly AI Governance Report presentations to the AI Review Committee (ARC) and executive leadership.
Failure to meet defined thresholds shall trigger corrective action workflows under AIMS-CAPA-001.
## 6. CONTINUAL IMPROVEMENT
AI governance objectives and KPIs shall be reviewed annually or upon material regulatory, operational, or technological change. Adjustments shall be documented and approved by the ARC.






# TILLI SOFTWARE
# AI COMPETENCY & AWARENESS POLICY
Document ID: AIMS-TRN-001
Version: 1.0
Owner: AI Governance Lead
Approved By: Board of Directors
Effective Date: [Insert Date]
Review Cycle: Annual
Framework Alignment: ISO/IEC 42001:2023 Clause 7.2

## 1. PURPOSE
This Policy defines the competency, training, and awareness requirements for personnel involved in the design, development, deployment, validation, monitoring, and oversight of Artificial Intelligence (AI) systems at Tilli Software. It ensures that AI-related responsibilities are performed by competent individuals in alignment with ISO/IEC 42001:2023 Clause 7.2.
## 2. SCOPE
This Policy applies to all employees, contractors, and third parties contributing to AI-enabled systems across Engineering, Product, Security, Compliance, Data, and Operations.
## 3. ROLE-BASED COMPETENCY REQUIREMENTS

| Role | Minimum Competency Requirements | Required Training |
| --- | --- | --- |
| AI Governance Lead | Understanding of AI risk frameworks, ISO 42001, regulatory exposure, and model governance principles | Annual AI Governance & Risk Training |
| Engineering Lead | Knowledge of AI system architecture, secure coding practices, validation controls, and monitoring | Secure AI Development Training (Annual) |
| Product Owner | Understanding of AI feature impact, business risk, and regulatory considerations | AI Product Risk Awareness Training (Annual) |
| Security Team | Knowledge of AI security threats, prompt injection risks, and monitoring controls | AI Security & Threat Modeling Training (Annual) |
| Independent Validator | Experience in model validation, statistical testing, bias analysis, and performance benchmarking | Advanced AI Model Validation Training (Annual) |

## 4. MANDATORY TRAINING REQUIREMENTS
- All AI contributors must complete onboarding AI governance training prior to production access.
- Annual refresher training is mandatory for all AI-related roles.
- Specialized training is required for personnel performing independent validation.
- Awareness communication regarding AI policy updates must be distributed organization-wide.
## 5. COMPETENCY ASSESSMENT & RECORDS
Competency shall be assessed through training completion records, attestation acknowledgments, and periodic review by the AI Governance Lead.
Training records shall be maintained in a controlled repository and retained for a minimum of five (5) years.
## 6. NON-COMPLIANCE
Personnel who fail to complete required training may have AI system access suspended until compliance is achieved.








# TILLI SOFTWARE
# AI CONTEXT & STAKEHOLDER ANALYSIS
Document ID: AIMS-CTX-001
Version: 1.0
Owner: AI Governance Lead
Approved By: Board of Directors
Effective Date: [Insert Date]
Review Cycle: Annual
Framework Alignment: ISO/IEC 42001:2023 Clauses 4.1 & 4.2

## 1. PURPOSE
This document defines the internal and external context within which Tilli Software’s Artificial Intelligence Management System (AIMS) operates. It identifies relevant interested parties, their expectations, and factors that influence AI governance decisions.
## 2. INTERNAL CONTEXT
- Multi-product AI-enabled technology environment (tilliX, tilliPay, Nudge, Beacon, tilliArc, XDEX, Analytics platforms);
- Combination of shared infrastructure and client-specific deployments;
- Integration with ISO 27001 Information Security Management System (ISMS);
- Use of internal AI systems (e.g., Jareis) and third-party AI providers;
- Client contractual AI restriction requirements;
- Financial and regulatory exposure related to AI-driven decision-making.
## 3. EXTERNAL CONTEXT
- Evolving global AI regulatory landscape (e.g., EU AI Act, sectoral regulations);
- Data protection and privacy laws (e.g., GDPR and similar frameworks);
- Industry expectations regarding ethical and responsible AI use;
- Client contractual obligations regarding AI transparency and usage restrictions;
- Market competitiveness and innovation pressure;
- Emerging AI security threats and adversarial risks.
## 4. INTERESTED PARTIES & EXPECTATIONS

| Interested Party | AI-Related Expectations / Requirements |
| --- | --- |
| Clients / Tenants | Secure, transparent AI usage; ability to request AI restriction; protection of sensitive data |
| Regulators | Compliance with applicable AI and data protection laws |
| Board of Directors | Effective risk oversight and governance controls |
| Employees | Clear guidance on responsible AI development and usage |
| End Users | Fair, unbiased, and reliable AI-driven functionality |
| Third-Party Vendors | Clear integration standards and compliance expectations |

## 5. DETERMINATION OF AIMS SCOPE
The Artificial Intelligence Management System (AIMS) applies to all AI-enabled systems developed, integrated, or deployed across Tilli Software products and client environments. AI-Restricted client deployments remain within governance scope but exclude AI feature activation.
## 6. REVIEW & UPDATE
This Context & Stakeholder Analysis shall be reviewed annually or upon significant regulatory, organizational, or technological changes.










# TILLI SOFTWARE
# AI MANAGEMENT REVIEW PROCEDURE
Document ID: AIMS-MR-001
Version: 1.0
Owner: AI Governance Lead
Approved By: Board of Directors
Effective Date: [Insert Date]
Review Cycle: Annual (with Quarterly Operational Reviews)
Framework Alignment: ISO/IEC 42001:2023 Clause 9.3

## 1. PURPOSE
This Procedure defines the formal management review process for Tilli Software’s Artificial Intelligence Management System (AIMS). It ensures executive oversight, strategic alignment, risk visibility, and continual improvement in accordance with ISO/IEC 42001:2023.
## 2. SCOPE
This procedure applies to executive leadership, the AI Review Committee (ARC), and the Board of Directors in their oversight of AI governance performance.
## 3. REVIEW FREQUENCY
Formal Management Review shall occur at least annually. Operational AI governance performance shall be reviewed quarterly through the Quarterly AI Governance Report.
## 4. MANAGEMENT REVIEW INPUTS
- Status of actions from previous management reviews;
- Changes in internal and external context (AIMS-CTX-001);
- AI Risk Register summary and risk posture trends;
- Validation compliance metrics;
- Incident trends and corrective action status;
- KPI performance results (AIMS-OBJ-001);
- Audit findings and remediation progress;
- Regulatory or contractual developments impacting AI systems;
- AI-Restricted tenant compliance verification results.
## 5. MANAGEMENT REVIEW OUTPUTS
- Decisions regarding AI governance improvements;
- Resource allocation decisions;
- Risk acceptance or escalation determinations;
- Approval of policy or procedural updates;
- Initiation of corrective or preventive actions;
- Strategic AI risk posture adjustments.
## 6. DOCUMENTATION & RECORDKEEPING
Management Review minutes shall be documented, approved, and retained in SharePoint. Action items shall be tracked to completion through designated governance workflows.
Records shall be retained for a minimum of seven (7) years.
## 7. ESCALATION & BOARD REPORTING
Material AI risks, regulatory exposure, or governance failures identified during Management Review shall be escalated to the Board of Directors.
# TILLI SOFTWARE
# CORRECTIVE & PREVENTIVE ACTION (CAPA) PROCEDURE
Document ID: AIMS-CAPA-001
Version: 1.0
Owner: AI Governance Lead
Approved By: Board of Directors
Effective Date: [Insert Date]
Review Cycle: Annual
Framework Alignment: ISO/IEC 42001:2023 Clause 10.1

## 1. PURPOSE
This Procedure defines the process for identifying, documenting, analyzing, correcting, and preventing nonconformities within Tilli Software’s Artificial Intelligence Management System (AIMS).
## 2. SCOPE
This procedure applies to all AI-related nonconformities, audit findings, control failures, policy violations, regulatory breaches, and material governance deviations.
## 3. NONCONFORMITY IDENTIFICATION
- Internal audit findings;
- External audit observations;
- AI incident investigations;
- KPI threshold breaches;
- Client complaints related to AI functionality;
- Unauthorized AI activation in restricted environments;
- Validation failures or monitoring breakdowns.
## 4. CORRECTIVE ACTION PROCESS
1. Log nonconformity in designated tracking system (e.g., Jira);
1. Assign responsible owner;
1. Conduct root cause analysis (e.g., 5 Whys or equivalent methodology);
1. Define corrective action plan;
1. Implement corrective action;
1. Verify effectiveness of corrective action;
1. Document closure approval.
## 5. PREVENTIVE ACTION
Preventive actions shall be initiated when trend analysis, monitoring results, or governance reviews indicate emerging risk patterns.
Preventive measures may include policy updates, control enhancements, additional training, or system redesign.
## 6. ESCALATION
Material nonconformities with regulatory, financial, or reputational impact shall be escalated to the AI Review Committee (ARC) and the Board of Directors.
## 7. DOCUMENTATION & RETENTION
CAPA records, including root cause analysis documentation and verification evidence, shall be retained for a minimum of five (5) years in the approved governance repository.
