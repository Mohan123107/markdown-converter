**ARTIFICIAL INTELLIGENCE GOVERNANCE POLICY**
**AND ARTIFICIAL INTELLIGENCE MANAGEMENT SYSTEM (AIMS) MANUAL**


| Organization: | Tilli Software |
| --- | --- |
| Document ID: | AIMS-001 (Consolidated) |
| Version: | 1.0 |
| Adopted By: | Board of Directors |
| Owner: | CTO (Operational) / AI Governance Lead (Oversight) |
| Effective Date: | 01-01-2026 |
| Review Cycle: | Quarterly |
| Reviewer: | Raja Vemuri |
| Applies To: | Engineering, Product, Security, Compliance, Data, Operations |
| Systems Referenced:

Drafted By: | GitHub, Jira, SharePoint, GitHub Actions, Datadog, AWS

Amit Kumar, Syed Shoeb, Suryakant Thombare |


# Table of Contents





















































































# PART A — ARTIFICIAL INTELLIGENCE GOVERNANCE POLICY
## ARTICLE I — PURPOSE
This Artificial Intelligence Governance Policy establishes the Artificial Intelligence Management System (AIMS) of Tilli Software (the “Company”).
Tilli recognizes that Artificial Intelligence (AI) systems introduce operational, ethical, legal, security, and reputational risks alongside significant innovation opportunities. This policy establishes the governance framework under which AI systems are designed, developed, deployed, and operated across the organization.
The purpose of this Policy is to:
1. Ensure responsible, secure, and compliant deployment of Artificial Intelligence systems;
1. Align Company practices with ISO/IEC 42001:2023;
1. Integrate AI governance within the Company’s ISO 27001 Information Security Management System (ISMS);
1. Mitigate financial, operational, legal, and reputational risks; and
1. Provide structured oversight by executive leadership and the Board.
## ARTICLE II — DEFINITIONS
**Artificial Intelligence System (AI System)**
Any software system utilizing machine learning, statistical modeling, algorithmic inference, or generative methods to produce predictions, classifications, recommendations, or automated decisions.
**High-Risk AI System**
An AI system capable of materially affecting financial transactions, fraud outcomes, customer eligibility, regulatory compliance, or consumer rights.
## ARTICLE III — SCOPE
This Policy applies to:
- All AI-enabled features and systems across Tilli products
- All internally developed AI systems (e.g., Jareis and other proprietary AI engines)
- All third-party AI integrations
- All environments (development, staging, production)
- All teams contributing to AI-powered systems, including Engineering, Product, Security, Data, and Operations
Products currently in scope include (but are not limited to):
- tilliX
- tilliPay
- Nudge
- Nudge Beacon
- Nudge CPaaS
- tilliArc
- XDEX
- Beacon
- Analytics and integration platforms
- Additional products as designated by leadership
## ARTICLE IV — GOVERNANCE STRUCTURE
### Section 4.1 AI Review Committee (ARC)
The Board establishes the AI Review Committee (ARC).
ARC Responsibilities:
- AI risk classification
- Approval of High-Risk AI deployments
- Oversight of validation
- Monitoring oversight
- Review of AI incidents
- Quarterly governance reporting
### Section 4.2 Roles and Accountability
Clear accountability is required for effective AI governance.

| Role | Responsibility |
| --- | --- |
| AI Governance Lead | Oversight of AI risk management, compliance alignment, and policy enforcement |
| Engineering Lead | Technical implementation, controls, and system integrity |
| Product Owner | Business justification, feature approval, and lifecycle oversight |
| Security Team | Security review, data protection validation |
| Compliance / Legal (if applicable) | Regulatory assessment and risk advisory |

Named individuals and reporting structures: Pending assignment by Executive Leadership.
No AI-enabled feature may be released to production without documented risk ownership and assigned accountability.
## ARTICLE V — GOVERNANCE PRINCIPLES
All AI systems at Tilli shall adhere to the following principles:
### 3.1 Responsible AI Use
AI systems must be designed and operated to minimize harm, prevent misuse, and protect stakeholders.
### 3.2 Risk-Based Approach
AI systems shall be assessed and governed proportionate to their impact and risk level.
### 3.3 Transparency
AI-enabled capabilities should be clearly identifiable where appropriate, and system behavior should be explainable to relevant stakeholders.
### 3.4 Human Oversight
AI outputs that influence critical operational, financial, or customer-facing decisions must allow for appropriate human review or override mechanisms.
### 3.5 Security and Data Protection
AI systems must comply with Tilli’s security and data governance standards, including access control, logging, and data protection requirements.
### 3.6 Continuous Improvement
AI systems shall be monitored, evaluated, and improved over time based on performance, risk trends, and incident learnings.
## ARTICLE VI — AI LIFECYCLE REQUIREMENTS
No AI System shall be deployed without completion of:
1. Formal intake and risk classification
1. Documented business and technical specifications
1. Validation (where required)
1. Security review
1. Monitoring configuration
1. Deployment approval
## ARTICLE VII — AI RISK MANAGEMENT
Each AI-enabled product must maintain an AI Risk Register that includes:
- Identified risks
- Risk description
- Likelihood and impact
- Mitigation strategy
- Residual risk
- Assigned owner
- Review date
Risks to consider include, but are not limited to:
- Hallucination and inaccurate outputs
- Bias and unfair outcomes
- Data leakage or privacy violations
- Prompt injection or adversarial misuse
- Model drift
- Security vulnerabilities
- Regulatory exposure
Risk registers must be reviewed:
- Before production release
- After significant feature changes
- At minimum quarterly
High-risk AI features require documented approval by the designated governance authority. Approval authority: Pending formal designation.
## ARTICLE VIII — REQUIRED DOCUMENTATION STANDARDS
Every AI-enabled product must maintain documented evidence covering:
- Business intent and functional requirements
- Technical architecture and AI integration design
- Technology stack and major dependencies
- Development workflow and code review practices
- Deployment and rollback processes
- AI risk assessment artifacts
- Human oversight mechanisms
- Feature-to-tenant mapping (where applicable)
- Data usage and data flow documentation
- Observability and monitoring approach
Documentation must be accessible, updated when significant changes occur, and traceable through version control.
## ARTICLE IX — MODEL VALIDATION
High-Risk AI Systems shall undergo independent validation prior to production deployment.
Validation shall include:
- Conceptual soundness review
- Data integrity assessment
- Performance benchmarking
- Bias testing
- Stress testing
- Monitoring verification
## ARTICLE X — OPERATIONAL OVERSIGHT AND MONITORING
AI-enabled systems must implement monitoring mechanisms appropriate to their risk level, including:
- Input and output logging (in compliance with privacy requirements)
- Error tracking
- Performance monitoring
- Alerting for abnormal or degraded behavior
- Periodic quality evaluation of AI outputs
Monitoring controls must be defined prior to production deployment.
## ARTICLE XI — INCIDENT MANAGEMENT
AI-related incidents must:
1. Be logged in the designated incident management system.
1. Undergo root cause analysis.
1. Include documented corrective and preventive actions.
1. Trigger updates to the AI Risk Register if new risks are identified.
Incident severity classification and response timelines: Pending definition by Security & Operations.
AI incidents shall be escalated within 24 hours where required by this AIMS.
## ARTICLE XII — CHANGE MANAGEMENT
Changes to AI systems — including model updates, prompt modifications, architecture changes, or new AI-enabled features — must:
- Undergo risk evaluation
- Be documented and version-controlled
- Follow established CI/CD approval processes
- Include rollback capability where feasible
Significant changes require governance review prior to release.
## ARTICLE XIII — THIRD-PARTY AI GOVERNANCE
When external AI providers are used:
- Vendor risks must be evaluated.
- Data sharing implications must be assessed.
- Contractual and compliance obligations must be reviewed.
- Security controls must be validated.
Vendor assessment procedure: Pending alignment with Procurement and Security.
## ARTICLE XIV — DATA GOVERNANCE FOR AI SYSTEMS
AI-enabled systems must document:
- Types of data processed
- Data sources
- Retention policies
- Access control mechanisms
Handling of sensitive or regulated data must comply with Tilli’s internal security and data protection standards.
Relevant policy references: Pending cross-reference to Information Security Policy.
## ARTICLE XV — PROHIBITED CONDUCT
The following activities are prohibited:
1. Use of regulated data without documented approval
1. Deployment outside formal AI intake workflow
1. Integration of unvetted third-party AI services
1. Circumvention of monitoring or security controls
1. Deployment of AI systems demonstrating unacceptable bias or discriminatory outcomes
Violations may result in disciplinary action.
## ARTICLE XVI — REPORTING AND OVERSIGHT
The ARC shall deliver a Quarterly AI Governance Report including:
- AI inventory summary
- Risk posture overview
- Incident analysis
- Regulatory developments
- Governance KPIs
Material AI incidents shall be escalated to the Board.
## ARTICLE XVII — AUDIT, REVIEW, AND CONTINUAL IMPROVEMENT
This AI Governance Policy shall be:
- Reviewed annually
- Reviewed upon significant regulatory or organizational change
- Updated when material AI capabilities are introduced
Tilli commits to continuous improvement through:
- Periodic reassessment of AI risks
- Monitoring performance trends
- Reviewing incident patterns
- Incorporating stakeholder feedback
- Updating governance practices as necessary
The Company shall conduct annual review of the AIMS including risk reassessment, policy updates, monitoring effectiveness review, and audit findings and remediation tracking.
## ARTICLE XVIII — DOCUMENT CONTROL
Version: 1.0
Owner: Pending Executive Assignment (Policy) / CTO (Procedure)
Effective Date: Pending Approval
Next Review Date: 12 months from effective date
Approved By: Pending Executive Approval
## ARTICLE XIX — BOARD APPROVAL
This Policy is adopted by resolution of the Board of Directors and shall remain in effect until amended or repealed.

| Approved on: | ________________________ |
| --- | --- |
| Chairperson: | ________________________ |


# PART B — ARTIFICIAL INTELLIGENCE GOVERNANCE PROCEDURE MANUAL
Document ID: AIP-PR-001
Owner: CTO
Applies To: Engineering, Product, Security, Compliance
Systems Referenced: GitHub, Jira, SharePoint, GitHub Actions, Datadog, AWS
## 1. PURPOSE
This Procedure Manual operationalizes the AI Governance Policy and defines the step-by-step lifecycle for AI systems.
## 2. AI SYSTEM LIFECYCLE (OPERATIONAL STEPS)
### 2.1 Stage 1 – AI Intake
Trigger: Jira Epic labeled `AI-INIT`
Required Inputs:
- Business objective
- Product impacted
- Data classification (PCI/PII/PHI/etc.)
- Tenant impact
- Jurisdictional exposure
- Decision impact level
ARC reviews intake and assigns risk classification.
### 2.2 Stage 2 – Risk Classification
Risk Levels:
- Low – No financial/customer impact
- Moderate – Customer-facing analytics or optimization
- High – Financial decisioning, fraud detection, regulatory impact
High-Risk systems require independent validation.
Risk Classification Form stored in SharePoint.
### 2.3 Stage 3 – Mandatory Documentation
Stored in: /AI Governance/{Product}/{System}/ (SharePoint)
Required:
- Business Requirements Document (BRD)
- Functional Specification
- Technical Specification
- Architecture Diagram
- Risk Classification Form
- Monitoring Plan
- Deployment Approval Record
Development may not begin without documentation folder creation.
### 2.4 Stage 4 – Development Controls
All AI code must:
- Reside in GitHub repositories
- Use protected branches
- Require pull request approval
- Include model version identifiers
- Log key outputs to Datadog
- Store secrets in AWS Secrets Manager
- Never hardcode credentials
### 2.5 Stage 5 – Model Validation (Moderate & High Risk)
Validation must include:
- Conceptual model review
- Data integrity assessment
- Reproducibility testing
- Performance benchmarking
- Bias and fairness testing
- False positive/negative analysis
- Stress testing (if financial impact)
- Monitoring threshold definition
High-Risk systems require independent validator.
Validation Report stored in SharePoint.
### 2.6 Stage 6 – Deployment Approval
Before production:
- Documentation complete
- Validation complete (if required)
- Security review complete
- ARC approval (High Risk)
- Rollback plan documented
Deployment only via GitHub Actions CI/CD.
### 2.7 Stage 7 – Monitoring & Observability
All AI systems must:
- Log model version and decision metadata
- Configure Datadog performance dashboards
- Define alert thresholds
- Implement drift monitoring (if applicable)
Monitoring review cadence:
- High Risk – Quarterly
- Moderate – Biannual
- Low – Annual
### 2.8 Stage 8 – Change Management
Trigger: Jira ticket labeled `AI-CHANGE`
Material changes include:
- New training dataset
- Model architecture change
- Jurisdiction expansion
- New financial impact logic
Requires:
- Updated risk assessment
- Updated documentation
- Re-validation (if required)
- ARC approval (if risk elevated)
### 2.9 Stage 9 – Incident Management
Trigger: Jira ticket labeled `AI-INCIDENT`
Required Actions:
1. Notify Security & Compliance within 24 hours
1. Assess financial and regulatory impact
1. Disable feature if necessary
1. Conduct root cause analysis
1. Document corrective actions
## 3. AI RISK REGISTER
Maintained in SharePoint.
Required Fields:
- System Name
- Model Version
- Risk Level
- Regulatory Exposure
- Data Classification
- Bias Risk
- Financial Impact
- Mitigation Controls
- Monitoring Controls
- Owner
- Review Dates
## 4. PROHIBITED USAGE ENFORCEMENT
Violations of AI Policy or Procedure may result in:
- Deployment suspension
- Security review
- Disciplinary action
- Vendor review
## 5. DEVELOPER ACKNOWLEDGMENT
All AI contributors must annually attest to:
- Compliance with AIMS
- Secure handling of regulated data
- Adherence to intake and validation requirements
- Prompt incident escalation
Records retained for minimum 5 years.
## 6. QUARTERLY AI GOVERNANCE REPORT
Prepared by ARC. Includes:
- AI system inventory
- Risk distribution
- Validation status
- Incident summary
- Drift/performance trends
- Regulatory updates
- Governance KPIs
Board escalation required for material AI incidents.
## 7. INTERNAL AUDIT
Annual audit shall verify:
- Risk classification accuracy
- Documentation completeness
- Validation compliance
- Monitoring effectiveness
- Incident response adequacy
- Developer acknowledgment compliance

# PART C — AI PRODUCT TECHNICAL DOCUMENTATION (NUDGE BEACON)
## 1. DOCUMENT OVERVIEW
This document provides a comprehensive technical and operational overview of Nudge Beacon, including its architecture, AI integration, development workflow, deployment process, governance artifacts, and monitoring controls.
This document supports compliance with the One Tilli AI Governance Policy and serves as the authoritative reference for engineering and audit purposes.
## 2. PRODUCT OVERVIEW
Product Name: Nudge Beacon
Category: Industry-Specific CRM Platform
Core Engine: Nudge CPaaS
AI System: Jareis (Just Another Rather Extremely Intelligent System)
Nudge Beacon is a CRM platform designed to support:
- Marketing workflows
- Sales workflows
- Customer Support workflows
- Native Oracle CC&B integration
- Planned expansion into ERP capabilities
AI functionality is primarily delivered through Jareis, which provides agent assistance and workflow intelligence.
## 3. BUSINESS CONTEXT & OBJECTIVES
### 3.1 Business Problem
[TBD – Define CRM inefficiencies, automation gaps, or operational pain points]
### 3.2 Objectives
- Improve agent productivity
- Reduce manual workload
- Provide intelligent workflow assistance
- Enhance CRM insights
- Enable scalable tenant-based deployments
### 3.3 Target Users
- Marketing Teams
- Sales Teams
- Customer Support Agents
- Administrators
## 4. AI SYSTEM DESCRIPTION
### 4.1 AI Component
Name: Jareis
Type: Internal AI-powered assistant
Purpose: Agent assistance and intelligent workflow augmentation
### 4.2 AI Functional Scope
- Suggest responses
- Automate repetitive tasks
- Provide contextual insights
- [TBD – Additional capabilities]
### 4.3 AI Invocation Flow (High-Level)
1. User performs action in Web UI.
1. Backend (Fastify API) processes request.
1. Jareis AI component invoked.
1. AI output processed and validated.
1. Response returned to user.
1. Logs recorded for monitoring.
[TBD – Insert detailed architecture diagram]
## 5. TECHNICAL ARCHITECTURE
### 5.1 System Components
Backend:
- Fastify (Node.js / TypeScript)
- Drizzle ORM
- PostgreSQL 16
Frontend:
- React (TypeScript)
Admin Portal:
- React
Database:
- PostgreSQL
Infrastructure:
- AWS ECS
- AWS ECR
- CI: GitHub Actions
### 5.2 Monorepo Structure
TilliBeacon/
├── apps/
│   ├── api/
│   ├── web/
│   └── admin-portal/
├── packages/
│   ├── db/
│   ├── sdk/
│   ├── shared/
│   └── ui/
├── docs/
├── scripts/
└── CLAUDE.md
### 5.3 AI & External Integrations
- Jareis (internal AI system)
- Oracle CC&B Integration
- [TBD – External model provider if applicable]
- [TBD – Vector database or embedding system if applicable]
## 6. TECHNOLOGY STACK
### 6.1 Development Stack
- Node.js
- TypeScript
- Fastify
- React
- TurboRepo
- pnpm
### 6.2 Database
- PostgreSQL 16
- Drizzle ORM
### 6.3 Governance & Tooling
- GitHub (Codeowners, branch protection rules)
- Jira (task tracking & traceability)
- CLAUDE.md (AI development guidance)
### 6.4 Infrastructure
- AWS ECS
- AWS ECR
- GitHub Actions (CI)
## 7. DEVELOPMENT & ONBOARDING
### 7.1 Local Setup
Install dependencies:
pnpm install
Setup database:
brew install postgresql@16
brew services start postgresql@16
psql postgres -c "CREATE DATABASE tilliccx;"
Configure environment:
cp .env.example .env
Run migrations:
pnpm db:push
Start services:
pnpm dev:start
API: http://localhost:5001
Web: http://localhost:4200
Full setup reference:
• docs/SETUP.md
• docs/PORTS.md
### 7.2 Environment Variable Management
- Development: .env based on .env.example
- Production: Managed via AWS Secrets Manager or ECS Task Definitions (Pending confirmation from DevOps)
- Secrets must never be committed to version control.
### 7.3 Coding Standards & Review Process
- Follow TypeScript strict typing
- Adhere to repository lint rules
- All PRs require review before merge
- Codeowners enforce review policies
- Branch protection enabled on main branches
AI-related code changes must:
- Be reviewed by designated AI engineering reviewers
- Include testing and validation where applicable
## 8. DEPLOYMENT & RELEASE MANAGEMENT
### 8.1 Continuous Integration
GitHub Actions pipeline includes:
- Build validation
- Lint checks
- Type checks
- Migration validation
### 8.2 Continuous Deployment
Deployment flow:
1. Docker image built
1. Pushed to AWS ECR
1. Deployed to AWS ECS
1. Service restarted
### 8.3 Rollback Strategy
- Revert to previous Docker image version
- Redeploy stable ECS task definition
Rollback authorization: Pending formal definition.
## 9. OBSERVABILITY & MONITORING
### 9.1 Logging
- API request logging
- Error logging
- AI invocation logging (privacy-compliant)
### 9.2 Monitoring
- Application health checks
- Performance monitoring
- Error rate tracking
Monitoring tools: Pending confirmation (CloudWatch / Datadog / Other).
### 9.3 Alerting
- Alerts configured for service downtime
- Alerts for abnormal error spikes
- [TBD – AI output anomaly alerts]
## 10. AI RISK REGISTER (INITIAL DRAFT)

| Risk | Impact | Mitigation | Owner |
| --- | --- | --- | --- |
| Hallucinated AI output | Incorrect CRM advice | Human review for high-impact workflows | Pending assignment |
| Data leakage | Exposure of sensitive data | Access controls & sanitized prompts | Pending assignment |
| Model drift | Reduced output quality | Periodic output review | Pending assignment |
| Prompt injection | Malicious input manipulation | Input validation & filtering | Pending assignment |

Risk review cadence: Quarterly minimum.
## 11. FEATURE & TENANT MAPPING
Each AI-enabled feature must document:
- Feature description
- AI involvement (Yes/No)
- Tenant enablement
- Risk classification
- Human oversight requirement
Example:

| Feature | AI Used | Tenants | Risk Level |
| --- | --- | --- | --- |
| Agent Assistance | Yes | [TBD] | Medium |
| Oracle CC&B Sync | No | [TBD] | Low |

## 12. ROADMAP & CHANGE GOVERNANCE
Feature lifecycle:
1. Requirement gathering
1. Feasibility review
1. Risk assessment
1. Proof of Concept
1. Validation
1. Production deployment
1. Monitoring & iteration
All new AI features require documented risk evaluation prior to release.
## 13. DOCUMENT CONTROL
Document Owner: Pending Engineering Assignment
Version: 1.0
Last Updated: [Insert Date]
Next Review: 12 months from approval
## WHAT THIS DOCUMENT ACHIEVES
- Serves as onboarding reference
- Captures technical architecture
- Documents AI integration
- Supports ISO 42001 governance requirements
- Creates audit traceability
- Provides operational clarity
