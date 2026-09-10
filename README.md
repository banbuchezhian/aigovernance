# AI Governance Portfolio Walkthrough

A comprehensive guide to AI governance implementation using three major frameworks: **NIST AI RMF**, **ISO/IEC 42001**, and **EU AI Act**. This portfolio includes real-world scenario examples showing how to apply governance across different industries and use cases.

## 📋 Contents

### Scenario Documentation
1. **`scenario-medsecure-health.md`** - Healthcare AI governance (reference example)
   - Staff Copilot (internal productivity AI)
   - Clinical Decision Agent (patient-facing AI)
   - Focus: Clinical safety, HIPAA/GDPR compliance, EU AI Act high-risk classification

2. **`scenario-1-finanalytics.md`** - Financial Services AI governance
   - Automated Underwriting Assistant (loan decision support)
   - Explainable Credit Decision System (customer-facing creditworthiness assessment)
   - Focus: Fairness, bias detection, lending law compliance, high-risk classification

3. **`scenario-2-retailai.md`** - E-commerce AI governance
   - Product Recommendation Engine (personalization, limited-risk)
   - Dynamic Pricing Optimizer (algorithmic pricing, high-risk)
   - Focus: Consumer protection, discrimination detection, transparency

### Reference Guides
- **`framework-mapping-guide.md`** - Cross-framework reference guide
  - Detailed explanation of each framework
  - Governance activity mappings
  - Checklist templates for implementation

---

## 🎯 Frameworks Covered

### NIST AI Risk Management Framework (RMF)
**Purpose**: Manage, measure, and govern AI-specific risks  
**Key Activities**: MAP → MEASURE → MANAGE → GOVERN

**What It Addresses**:
- Risk categorization and assessment
- Performance metrics and thresholds
- Fairness and bias detection
- Stakeholder impact analysis
- Mitigation control selection

**When to Use**: Risk assessment, metrics definition, control prioritization

---

### ISO/IEC 42001 - AI Management Systems
**Purpose**: Establish systematic AI governance across the organization  
**Key Elements**: Policy, processes, documentation, roles, continuous improvement

**What It Addresses**:
- AI governance structure and accountability
- Resource and competence management
- AI system inventory and lifecycle
- Performance monitoring and audits
- Improvement processes

**When to Use**: Building governance infrastructure, policy documentation, audit readiness

---

### EU AI Act
**Purpose**: Regulatory compliance for AI systems in EU markets  
**Key Mechanism**: Risk-tier classification with proportional obligations

**Risk Tiers**:
- **Prohibited**: Unacceptable risk systems (banned)
- **High-Risk**: Subject to conformity assessment, documentation, monitoring
- **Limited Risk**: Transparency requirements
- **Minimal/No Risk**: No specific AI Act requirements

**What It Addresses**:
- Risk classification and compliance obligations
- Technical documentation requirements
- Conformity assessment procedures
- Transparency and explainability
- Audit trail and record-keeping

**When to Use**: Regulatory compliance, risk tier determination, documentation checklist

---

## 🔄 How Frameworks Work Together

```
NIST AI RMF
    ↓ (provides risk assessment)
EU AI Act Risk Tier Classification
    ↓ (determines regulatory tier)
ISO 42001 AIMS Implementation
    ↓ (builds governance infrastructure)
Ongoing Monitoring & Improvement
```

**Example Flow**:
1. **MAP (NIST)**: Identify clinical decision AI system and stakeholders
2. **Classify (EU AI Act)**: Determine High-Risk tier due to patient safety impact
3. **Establish (ISO 42001)**: Create clinical AI governance policy and controls
4. **Measure (NIST)**: Define fairness metrics, accuracy thresholds, bias detection
5. **Monitor**: Track metrics, conduct quarterly reviews, improve continuously

---

## 📊 Scenario Comparison Matrix

| Aspect | MedSecure Health | FinAnalytics Corp | RetailAI Systems |
|--------|------------------|-------------------|------------------|
| **Industry** | Healthcare | Financial Services | E-commerce |
| **Primary Risk** | Patient Safety | Discrimination | Consumer Harm |
| **EU AI Act Tier** | High-Risk | High-Risk | Mixed (Limited + High) |
| **Key Compliance** | HIPAA, GDPR | Fair Lending, GDPR | Consumer Protection, GDPR |
| **NIST Focus** | Clinical validity, safety | Fairness, bias | Price discrimination |
| **ISO Focus** | Clinical controls, AIMS | Fairness governance | Personalization governance |

---

## 🚀 Getting Started

### For New AI Governance Programs
1. Read `framework-mapping-guide.md` for framework overview
2. Select the scenario most similar to your use case
3. Use the scenario as a template for your system
4. Follow the governance checklist in the guide

### For Existing Programs
1. Map current practices to each framework using the guide
2. Identify gaps in ISO 42001 AIMS implementation
3. Conduct NIST AI RMF risk assessment for each system
4. Validate EU AI Act compliance and classification

### For Audit & Compliance
1. Review relevant scenario for your industry
2. Use the framework-mapping-guide checklist
3. Prepare artifacts list for each phase
4. Schedule assessment with internal/external auditors

---

## 📁 Artifact Types Referenced

### Governance Artifacts
- AI Governance Policy
- Risk Assessment Reports
- Classification Decisions (NIST + EU AI Act)

### Technical Artifacts
- Model Cards
- Data Impact Assessments
- System Architecture Documentation

### Compliance Artifacts
- Fairness Audit Reports
- Conformity Assessment Reports
- Audit Trail Logs

### Operational Artifacts
- Monitoring Dashboards
- Incident Response Logs
- Training Records

---

## 🔗 Key Concepts

### Fairness & Bias
The prevention of discriminatory outcomes based on protected characteristics. Critical for lending, hiring, and consumer-facing AI.

**How each framework addresses it**:
- **NIST**: Define fairness metrics and bias thresholds
- **ISO 42001**: Create bias testing and monitoring processes
- **EU AI Act**: Mandatory bias mitigation for high-risk systems

### Explainability
The ability for users/stakeholders to understand why an AI system made a decision.

**How each framework addresses it**:
- **NIST**: Measure explainability quality
- **ISO 42001**: Document explanation mechanisms and validation
- **EU AI Act**: Require transparency proportional to risk tier

### Human Oversight
Mechanisms to ensure humans can understand, review, and override AI decisions.

**How each framework addresses it**:
- **NIST**: Map human roles and decision authority
- **ISO 42001**: Define escalation and review procedures
- **EU AI Act**: Mandate human oversight for high-risk systems

### Monitoring & Continuous Improvement
Ongoing tracking of AI system performance and risk metrics.

**How each framework addresses it**:
- **NIST**: Establish performance dashboards and KPIs
- **ISO 42001**: Define review frequency and improvement triggers
- **EU AI Act**: Require monitoring logs and incident reporting

---

## 📚 Additional Resources

### NIST AI RMF
- Full Framework: https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf
- Resource Center: https://airc.nist.gov/

### ISO/IEC 42001
- Standard Text: https://www.iso.org/standard/81230.html
- Implementation Guides: ISO provides guidance documents

### EU AI Act
- Regulation Text: https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689
- European Commission AI Office: https://digital-strategy.ec.europa.eu/en/policies/ai-act

### Related Regulations
- GDPR: https://gdpr-info.eu/
- CCPA: https://oag.ca.gov/privacy/ccpa
- Fair Lending Laws: https://www.federalreserve.gov/aboutthefed/boardmeetings/fair-lending-laws.htm

---

## 💡 Best Practices

### Governance Setup
✓ Assign clear AI governance ownership and accountability  
✓ Classify all AI systems using NIST and EU AI Act frameworks  
✓ Document governance policies and procedures in ISO 42001 format  
✓ Establish metrics dashboards for ongoing monitoring  

### Risk Management
✓ Conduct comprehensive risk assessments for each AI system  
✓ Define fairness metrics and baseline measurements  
✓ Implement bias detection and mitigation controls  
✓ Plan for continuous model monitoring and retraining  

### Compliance
✓ Map all systems to EU AI Act risk tiers with documentation  
✓ Maintain complete audit trails for high-risk systems  
✓ Conduct regular third-party assessments  
✓ Keep governance documentation current and accessible  

### Transparency
✓ Clearly communicate AI use to stakeholders  
✓ Provide explainability proportional to system risk  
✓ Offer human review and appeal mechanisms  
✓ Publish transparency reports on AI system performance  

---

## 📝 Version Control

This portfolio is maintained in GitHub with the following structure:
```
/aigovernance/
├── README.md
├── .gitignore
├── CONTRIBUTING.md
├── LICENSE
│
├── docs/
│   ├── framework-mapping-guide.md
│   └── governance-checklist.md
│
├── scenarios/
│   ├── scenario-medsecure-health.md
│   ├── scenario-1-finanalytics.md
│   └── scenario-2-retailai.md
│
├── templates/
│   └── model-card-template.md
│
├── examples/
│   ├── healthcare/
│   ├── financial/
│   └── ecommerce/
│
├── resources/
├── tools/
└── .github/
    └── ISSUE_TEMPLATE/
```

---

## 🤝 Contributing

To suggest improvements or add scenarios:
1. Create a new branch for your scenario
2. Follow the same structure as existing scenarios
3. Ensure all three frameworks are mapped
4. Submit a pull request with description

---

## 📄 License

Creative Commons 4.0

---

## 📧 Contact & Support

For questions about this governance portfolio:
- Create an issue in the GitHub repository
- Reference the specific scenario or framework section
- Include your use case for context

---

*Last Updated**: September 2026  
*Framework Versions**: NIST AI RMF 1.0 | ISO/IEC 42001:2023 | EU AI Act (2024/1689)
=======

