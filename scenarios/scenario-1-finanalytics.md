# Scenario 1: FinAnalytics AI Credit Scoring System

## Company Overview
**Organization:** FinAnalytics Corp  
**Industry:** Financial Services  
**Region:** EU + USA  
**Compliance Requirements:** GDPR + Fair Lending Laws + Upcoming EU AI Act (High-Risk Classification)

---

## AI Projects

### Project A: Automated Underwriting Assistant
Approved AI tool for loan eligibility screening using machine learning models trained on historical loan data to predict default risk and support loan officers in initial assessment.

### Project B: Explainable Credit Decision System
Real-time AI system providing transparent credit scoring with explainability features, bias detection, and human-in-the-loop review for all credit decisions above specified thresholds.

---

## Framework Mapping

| Framework | What It Helps FinAnalytics Ask | Automated Underwriting Assistant | Explainable Credit Decision System |
|-----------|-------------------------------|----------------------------------|-------------------------------------|
| **NIST AI RMF** | Have we governed, measured, and managed AI risk across our credit products? | Map model performance, fairness metrics, data quality, and stakeholder impact. Establish baseline metrics for bias across protected classes. | Measure explainability quality, human override rates, decision consistency, and outcome disparities by demographic group. |
| **ISO/IEC 42001** | Is AI governance structured, resourced, documented, measured, and improved? | Define AI governance policy for underwriting, establish model inventory, assign owners, and establish quarterly review cadence. | Create formal AIMS (AI Management System) controls covering model lifecycle, performance monitoring, fairness audits, and continuous improvement processes. |
| **EU AI Act** | What risk tier, role, and evidence obligations apply to our credit decisions? | Classify as High-Risk system (prohibited if discriminatory risk). Document training data, implement bias testing, maintain detailed decision logs, and establish human oversight for borderline cases. | Establish comprehensive documentation requirements, implement audit trail logging, conduct conformity assessments, and maintain technical file with test results and validation reports. |

---

## Governance Artifacts Required

- **Model Card**: Document model architecture, training data, performance metrics, limitations
- **Data Impact Assessment**: GDPR/CCPA privacy assessment for training and operational data
- **Fairness Audit Report**: Demographic parity, disparate impact analysis, bias mitigation strategies
- **Human Review Protocol**: Decision review thresholds, escalation procedures, appeal process
- **Conformity Assessment**: EU AI Act technical documentation and compliance checklist
- **Risk Management Plan**: Ongoing monitoring, incident response, model drift detection

---

## Key Governance Considerations

1. **Data & Fairness**: Training data must be regularly audited for historical bias; fairness metrics tracked continuously
2. **Explainability**: Credit decisions must be explainable to applicants per GDPR Article 22 and Fair Lending requirements
3. **Human Oversight**: Mandatory human review for all decisions; clear escalation for model disagreements
4. **Audit & Documentation**: Maintain complete audit trail; quarterly third-party fairness audits for high-risk decisions
5. **Transparency**: Clear communication of AI use in lending process; dispute resolution mechanisms in place
