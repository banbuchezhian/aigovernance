# AI Governance Framework Mapping Guide

## Overview
This guide provides a unified approach to AI governance across three major frameworks:
- **NIST AI Risk Management Framework (RMF)** - Risk-centric governance
- **ISO/IEC 42001** - AI Management System structure
- **EU AI Act** - Regulatory compliance requirements

---

## Framework Characteristics

### NIST AI RMF
**Purpose**: Manage, measure, and govern AI-specific risks  
**Approach**: Principles-based, risk categorization, context-aware  
**Key Activities**: 
- MAP: Understand AI system, context, risks
- MEASURE: Develop metrics for performance and risk
- MANAGE: Implement controls and mitigation strategies
- GOVERN: Integrate into organizational processes

**Best For**: Risk assessment, metrics definition, control selection

---

### ISO/IEC 42001
**Purpose**: Establish formal AI management system  
**Approach**: Process-based, systematic documentation, continuous improvement  
**Key Elements**:
- AI governance and organization
- Resource management
- Competence and awareness
- Operational planning and control
- Performance evaluation and improvement

**Best For**: Governance structure, policy documentation, audit readiness

---

### EU AI Act
**Purpose**: Regulatory compliance for AI systems in EU/EEA  
**Approach**: Risk-tier classification, regulatory obligations by risk level  
**Risk Tiers**:
- **Prohibited**: Systems creating unacceptable risk
- **High-Risk**: Subject to conformity assessment, documentation, monitoring
- **Limited Risk**: Transparency requirements
- **Minimal/No Risk**: No specific requirements

**Best For**: Regulatory classification, compliance checklist, audit trail

---

## Use Case Scenarios

### Scenario 1: MedSecure Health (Healthcare AI)
| Aspect | Focus |
|--------|-------|
| **Industry** | Healthcare |
| **Systems** | Staff Copilot (internal productivity) + Clinical Decision Agent (patient-facing) |
| **Primary Compliance** | HIPAA + EU GDPR + EU AI Act (High-Risk) |
| **NIST Focus** | Risk assessment for clinical impact, fairness in treatment recommendations |
| **ISO Focus** | Clinical AI governance, AIMS for medical device regulation |
| **EU AI Act** | High-Risk classification; requires conformity assessment, clinical validation |

---

### Scenario 2: FinAnalytics Corp (Financial Services AI)
| Aspect | Focus |
|--------|-------|
| **Industry** | Financial Services / Lending |
| **Systems** | Automated Underwriting (decision support) + Explainable Credit System (customer-facing) |
| **Primary Compliance** | GDPR + Fair Lending Laws + EU AI Act (High-Risk) |
| **NIST Focus** | Fairness metrics, bias detection, stakeholder impact assessment |
| **ISO Focus** | Credit AI governance policy, model lifecycle management, fairness audits |
| **EU AI Act** | High-Risk (lending decisions); prohibited if discriminatory; requires detailed documentation |

---

### Scenario 3: RetailAI Systems (E-commerce AI)
| Aspect | Focus |
|--------|-------|
| **Industry** | E-commerce / Retail |
| **Systems** | Product Recommendation Engine (Limited Risk) + Dynamic Pricing (High-Risk) |
| **Primary Compliance** | GDPR + CCPA + Consumer Protection + EU AI Act |
| **NIST Focus** | Filter bubble risk, price discrimination detection, consumer harm prevention |
| **ISO Focus** | Personalization system governance, pricing algorithm management, fairness controls |
| **EU AI Act** | Pricing classified as High-Risk; recommendations as Limited Risk; discrimination detection required |

---

## Cross-Framework Governance Activities

### Governance & Organization (ISO 42001 + NIST MAP)
**What to Document**:
- AI governance structure and accountability
- Risk categorization and classification (NIST + EU AI Act tiers)
- Stakeholder identification
- Decision authority and escalation paths

**Example**:
> *"Our organization has established an AI Governance Committee reporting to the Chief Risk Officer. All AI systems are classified using both NIST AI RMF categories and EU AI Act risk tiers. High-risk systems require executive steering committee approval before deployment."*

---

### Risk Assessment & Classification (NIST MAP + EU AI Act)
**What to Document**:
- NIST AI RMF risk mapping across four dimensions (impact, performance, security, fairness)
- EU AI Act risk tier determination with rationale
- Stakeholder impact analysis
- Intended vs. foreseeable use cases

**Example**:
> *"The clinical decision agent is mapped as High-Risk under EU AI Act due to potential patient safety impact. NIST RMF impact assessment identifies risks in: performance (diagnostic accuracy), fairness (demographic bias), and security (data privacy). Mitigating controls established in ISO 42001 AIMS."*

---

### Data Governance (ISO 42001 + NIST MEASURE)
**What to Document**:
- Training data inventory and provenance
- Data quality metrics and thresholds
- Bias audits and demographic representation analysis
- Data retention and deletion policies

**Example**:
> *"All training datasets are documented in our AI model registry. Quarterly fairness audits compare model performance across demographic groups. Data retention policies comply with GDPR Article 17 (right to erasure) and CCPA deletion requirements."*

---

### Model Governance (ISO 42001 Operational Control)
**What to Document**:
- Model card with technical specifications
- Performance monitoring metrics and SLAs
- Validation and testing protocols
- Human review thresholds and escalation procedures

**Example**:
> *"Each production model has a model card documenting architecture, training data, performance metrics, and known limitations. Weekly performance monitoring tracks accuracy, fairness, and drift. Models triggering drift alerts undergo retraining evaluation within 30 days."*

---

### Monitoring & Audit (NIST MEASURE + GOVERN)
**What to Document**:
- KPIs and metrics dashboard
- Audit procedures and frequency
- Third-party assessment plans
- Incident reporting and response procedures

**Example**:
> *"Our AI system monitoring dashboard tracks 25+ metrics covering performance, fairness, and security. Monthly internal audits assess compliance with governance policies. Annual third-party audits validate control effectiveness for ISO 42001 and EU AI Act conformity."*

---

### Transparency & Explainability (EU AI Act + NIST)
**What to Document**:
- How users understand AI involvement
- Explainability mechanisms and quality
- Opt-out and human review procedures
- Decision appeal and remedy processes

**Example**:
> *"Users receive clear notifications when AI influences recommendations. Explainability features show key factors influencing decisions. Users may request human review of any AI-driven decision. Feedback mechanisms inform ongoing fairness improvements."*

---

## Governance Checklist Template

For each AI system, complete:

### Phase 1: Classification & Planning
- [ ] NIST AI RMF risk categorization complete
- [ ] EU AI Act risk tier determined
- [ ] Stakeholder impact assessment documented
- [ ] Governance owner assigned

### Phase 2: Documentation & Controls
- [ ] ISO 42001 AIMS policy and procedures drafted
- [ ] Risk mitigation controls identified
- [ ] Data governance framework defined
- [ ] Model governance procedures documented

### Phase 3: Implementation & Validation
- [ ] Training data audited for bias and quality
- [ ] Model validation completed against specifications
- [ ] Fairness metrics baseline established
- [ ] Monitoring dashboards deployed

### Phase 4: Monitoring & Improvement
- [ ] Audit and review schedule established
- [ ] Incident response procedures tested
- [ ] Continuous improvement process defined
- [ ] Stakeholder feedback mechanisms in place

---

## References & Resources

- NIST AI Risk Management Framework: https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf
- ISO/IEC 42001:2023 AI Management Systems: https://www.iso.org/standard/81230.html
- EU AI Act Text: https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689
- GDPR: https://gdpr-info.eu/
- CCPA: https://oag.ca.gov/privacy/ccpa
