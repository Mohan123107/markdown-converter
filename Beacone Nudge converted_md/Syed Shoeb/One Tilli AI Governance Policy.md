# 📄 One Tilli AI Governance Policy
*(Aligned with ISO/IEC 42001 AI Management System Principles)*

## 1. Purpose
Tilli recognizes that Artificial Intelligence (AI) systems introduce operational, ethical, legal, security, and reputational risks alongside significant innovation opportunities.
This policy establishes the governance framework under which AI systems are designed, developed, deployed, and operated across the organization. It defines accountability, risk management expectations, documentation standards, and oversight mechanisms to ensure responsible and sustainable AI adoption.
This policy forms the foundation of Tilli’s AI Management System and supports alignment with ISO/IEC 42001 principles.

## 2. Scope
This policy applies to:
All AI-enabled features and systems across Tilli products
All internally developed AI systems (e.g., Jareis and other proprietary AI engines)
All third-party AI integrations
All environments (development, staging, production)
All teams contributing to AI-powered systems, including Engineering, Product, Security, Data, and Operations
Products currently in scope include (but are not limited to):
Nudge
XDEX
tilliX
tilliArc
Beacon
Additional products as designated by leadership

## 3. Governance Principles
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

## 4. Roles and Accountability
Clear accountability is required for effective AI governance.
The following roles are responsible for AI oversight:

| Role | Responsibility |
| --- | --- |
| AI Governance Lead | Oversight of AI risk management, compliance alignment, and policy enforcement |
| Engineering Lead | Technical implementation, controls, and system integrity |
| Product Owner | Business justification, feature approval, and lifecycle oversight |
| Security Team | Security review, data protection validation |
| Compliance / Legal (if applicable) | Regulatory assessment and risk advisory |

Named individuals and reporting structures: **Pending assignment by Executive Leadership**
No AI-enabled feature may be released to production without documented risk ownership and assigned accountability.

## 5. AI Lifecycle Governance
All AI-enabled initiatives must follow a structured lifecycle:
Business requirement definition
Feasibility and impact assessment
AI risk assessment
Technical design and review
Development and validation
Deployment approval
Monitoring and observability
Periodic review and improvement
A documented risk assessment is mandatory prior to production deployment.

## 6. AI Risk Management
Each AI-enabled product must maintain an AI Risk Register that includes:
Identified risks
Risk description
Likelihood and impact
Mitigation strategy
Residual risk
Assigned owner
Review date
Risks to consider include, but are not limited to:
Hallucination and inaccurate outputs
Bias and unfair outcomes
Data leakage or privacy violations
Prompt injection or adversarial misuse
Model drift
Security vulnerabilities
Regulatory exposure
Risk registers must be reviewed:
Before production release
After significant feature changes
At minimum quarterly
High-risk AI features require documented approval by the designated governance authority. Approval authority: **Pending formal designation**

## 7. Required Documentation Standards
To ensure consistency and audit readiness, every AI-enabled product must maintain documented evidence covering:
Business intent and functional requirements
Technical architecture and AI integration design
Technology stack and major dependencies
Development workflow and code review practices
Deployment and rollback processes
AI risk assessment artifacts
Human oversight mechanisms
Feature-to-tenant mapping (where applicable)
Data usage and data flow documentation
Observability and monitoring approach
This policy does not replace product documentation; it mandates its existence and maintenance.
Documentation must be:
Accessible to relevant stakeholders
Updated when significant changes occur
Traceable through version control

## 8. Operational Oversight and Monitoring
AI-enabled systems must implement monitoring mechanisms appropriate to their risk level, including:
Input and output logging (in compliance with privacy requirements)
Error tracking
Performance monitoring
Alerting for abnormal or degraded behavior
Periodic quality evaluation of AI outputs
Monitoring controls must be defined prior to production deployment.

## 9. Incident Management
AI-related incidents must:
Be logged in the designated incident management system.
Undergo root cause analysis.
Include documented corrective and preventive actions.
Trigger updates to the AI Risk Register if new risks are identified.
Incident severity classification and response timelines: **Pending definition by Security & Operations**

## 10. Change Management
Changes to AI systems — including model updates, prompt modifications, architecture changes, or new AI-enabled features — must:
Undergo risk evaluation
Be documented and version-controlled
Follow established CI/CD approval processes
Include rollback capability where feasible
Significant changes require governance review prior to release.

## 11. Third-Party AI Governance
When external AI providers are used:
Vendor risks must be evaluated.
Data sharing implications must be assessed.
Contractual and compliance obligations must be reviewed.
Security controls must be validated.
Vendor assessment procedure: **Pending alignment with Procurement and Security**

## 12. Data Governance for AI Systems
AI-enabled systems must document:
Types of data processed
Data sources
Retention policies
Access control mechanisms
Handling of sensitive or regulated data must comply with Tilli’s internal security and data protection standards.
Relevant policy references: **Pending cross-reference to Information Security Policy**

## 13. Audit, Review, and Continuous Improvement
This AI Governance Policy shall be:
Reviewed annually
Reviewed upon significant regulatory or organizational change
Updated when material AI capabilities are introduced
Tilli commits to continuous improvement through:
Periodic reassessment of AI risks
Monitoring performance trends
Reviewing incident patterns
Incorporating stakeholder feedback
Updating governance practices as necessary

## 14. Document Control
Version: 1.0 Owner: Pending Executive Assignment Effective Date: Pending Approval Next Review Date: 12 months from effective date Approved By: Pending Executive Approval

# Final Note
This policy establishes governance requirements for AI systems across Tilli. Product-specific technical documentation must be maintained in accordance with this policy and is subject to governance oversight.
