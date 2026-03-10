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
