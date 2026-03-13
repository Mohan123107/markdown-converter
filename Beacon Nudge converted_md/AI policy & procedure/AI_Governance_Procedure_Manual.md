# ARTIFICIAL INTELLIGENCE GOVERNANCE PROCEDURE MANUAL

**Organization:** Tilli Software  
**Document ID:** AIP-PR-001  
**Owner:** CTO  
**Applies To:** Engineering, Product, Security, Compliance  
**Systems Referenced:** GitHub, Jira, SharePoint, GitHub Actions, Datadog, AWS  

---

# 1. PURPOSE

This Procedure Manual operationalizes the AI Governance Policy and defines the step-by-step lifecycle for AI systems.

---

# 2. AI SYSTEM LIFECYCLE

---

## 2.1 Stage 1 – AI Intake

Trigger: Jira Epic labeled `AI-INIT`

Required Inputs:
- Business objective
- Product impacted
- Data classification (PCI/PII/PHI/etc.)
- Tenant impact
- Jurisdictional exposure
- Decision impact level

ARC reviews intake and assigns risk classification.

---

## 2.2 Stage 2 – Risk Classification

### Risk Levels

Low – No financial/customer impact  
Moderate – Customer-facing analytics or optimization  
High – Financial decisioning, fraud detection, regulatory impact

High-Risk systems require independent validation.

Risk Classification Form stored in SharePoint.

---

## 2.3 Stage 3 – Mandatory Documentation

Stored in:

`/AI Governance/{Product}/{System}/`

Required:

- Business Requirements Document (BRD)
- Functional Specification
- Technical Specification
- Architecture Diagram
- Risk Classification Form
- Monitoring Plan
- Deployment Approval Record

Development may not begin without documentation folder creation.

---

## 2.4 Stage 4 – Development Controls

All AI code must:

- Reside in GitHub repositories
- Use protected branches
- Require pull request approval
- Include model version identifiers
- Log key outputs to Datadog
- Store secrets in AWS Secrets Manager
- Never hardcode credentials

---

## 2.5 Stage 5 – Model Validation (Moderate & High Risk)

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

---

## 2.6 Stage 6 – Deployment Approval

Before production:

- Documentation complete
- Validation complete (if required)
- Security review complete
- ARC approval (High Risk)
- Rollback plan documented

Deployment only via GitHub Actions CI/CD.

---

## 2.7 Stage 7 – Monitoring & Observability

All AI systems must:

- Log model version and decision metadata
- Configure Datadog performance dashboards
- Define alert thresholds
- Implement drift monitoring (if applicable)

Monitoring review cadence:
- High Risk – Quarterly
- Moderate – Biannual
- Low – Annual

---

## 2.8 Stage 8 – Change Management

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

---

## 2.9 Stage 9 – Incident Management

Trigger: Jira ticket labeled `AI-INCIDENT`

Required Actions:
1. Notify Security & Compliance within 24 hours
2. Assess financial and regulatory impact
3. Disable feature if necessary
4. Conduct root cause analysis
5. Document corrective actions

---

# 3. AI RISK REGISTER

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

---

# 4. PROHIBITED USAGE ENFORCEMENT

Violations of AI Policy or Procedure may result in:

- Deployment suspension
- Security review
- Disciplinary action
- Vendor review

---

# 5. DEVELOPER ACKNOWLEDGMENT

All AI contributors must annually attest to:

- Compliance with AIMS
- Secure handling of regulated data
- Adherence to intake and validation requirements
- Prompt incident escalation

Records retained for minimum 5 years.

---

# 6. QUARTERLY AI GOVERNANCE REPORT

Prepared by ARC.

Includes:

- AI system inventory
- Risk distribution
- Validation status
- Incident summary
- Drift/performance trends
- Regulatory updates
- Governance KPIs

Board escalation required for material AI incidents.

---

# 7. INTERNAL AUDIT

Annual audit shall verify:

- Risk classification accuracy
- Documentation completeness
- Validation compliance
- Monitoring effectiveness
- Incident response adequacy
- Developer acknowledgment compliance

---

# END OF PROCEDURE MANUAL
