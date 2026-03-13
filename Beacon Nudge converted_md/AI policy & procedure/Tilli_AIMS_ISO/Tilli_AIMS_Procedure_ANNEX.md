# TILLI SOFTWARE
# ARTIFICIAL INTELLIGENCE GOVERNANCE PROCEDURE MANUAL
Volume II — AI Governance Procedures
Document ID: AIP-PR-001 (Consolidated)
Version: 1.0
Owner: CTO
Applies To: Engineering, Product, Security, Compliance, Data, Operations
Systems Referenced: GitHub, Jira, SharePoint, GitHub Actions, Datadog, AWS

# TABLE OF CONTENTS


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
