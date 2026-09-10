# AI Governance Policy Template

**Organization Name**: [Your Organization]  
**Policy Title**: Artificial Intelligence Governance Policy  
**Effective Date**: [YYYY-MM-DD]  
**Last Updated**: [YYYY-MM-DD]  
**Version**: 1.0  
**Owner**: [Chief Risk Officer / AI Governance Officer]  
**Approval**: [Board / Executive Committee]

---

## 1. Purpose & Scope

### 1.1 Purpose
This policy establishes the governance framework for the development, deployment, and monitoring of Artificial Intelligence (AI) systems to:
- Ensure responsible AI development and deployment
- Manage AI-related risks
- Maintain compliance with applicable regulations
- Protect stakeholder interests and organizational reputation
- Enable trustworthy AI innovation

### 1.2 Scope
This policy applies to:
- All AI and machine learning systems developed or deployed by [Organization]
- All employees, contractors, and third-party vendors involved in AI development or deployment
- Systems affecting customers, patients, employees, or other stakeholders
- Systems processing sensitive data (personal data, health information, financial data, etc.)

**Exclusions** (if any):
- Simple rule-based systems without machine learning
- Pre-built tools with no customization
- [Other exclusions specific to your organization]

---

## 2. Definitions

### 2.1 Key Terms

**Artificial Intelligence (AI)**: A system capable of performing tasks that typically require human intelligence, including learning from data, recognizing patterns, understanding language, or making decisions.

**Machine Learning (ML)**: A subset of AI that enables systems to learn and improve from experience without being explicitly programmed.

**Model**: A mathematical representation trained on data to make predictions or decisions.

**Algorithm**: A step-by-step procedure or set of rules for performing a task or solving a problem.

**High-Risk AI System**: An AI system that could significantly impact fundamental rights, safety, or well-being of individuals or stakeholders (per EU AI Act or organization definition).

**Fairness**: The absence of discriminatory bias; treating similar individuals similarly regardless of protected characteristics.

**Bias**: Systematic error or prejudice that causes AI system to treat certain groups unfairly.

**Explainability**: The ability to explain why an AI system made a specific decision in understandable terms.

**Monitoring**: Ongoing observation and measurement of AI system performance and behavior.

**Drift**: Degradation in model performance over time due to changes in data distribution or system environment.

### 2.2 Framework Definitions

**NIST AI RMF**: National Institute of Standards and Technology AI Risk Management Framework (MAP → MEASURE → MANAGE → GOVERN)

**ISO/IEC 42001**: International standard for AI Management Systems

**EU AI Act**: Regulation (EU) 2024/1689 establishing rules on AI

---

## 3. Governance Structure & Roles

### 3.1 Organizational Structure

**AI Governance Committee** (Executive Level)
- **Chair**: Chief Risk Officer / Chief Technology Officer
- **Members**: 
  - Chief Medical Officer (if healthcare)
  - Chief Information Officer
  - Chief Data Officer
  - Compliance Officer
  - Legal Counsel
  - Business Unit Heads
- **Responsibilities**:
  - AI strategy and policy approval
  - High-risk system oversight
  - Regulatory compliance monitoring
  - Escalation for critical issues
  - Board reporting

**AI Governance Office** (Operational Level)
- **Head**: AI Governance Officer
- **Team Members**:
  - AI Risk Analysts
  - Data Governance Specialist
  - Compliance Manager
  - Model Validators
- **Responsibilities**:
  - Day-to-day governance execution
  - System classification and assessment
  - Risk monitoring and reporting
  - Audit and compliance tracking

### 3.2 Roles & Responsibilities

| Role | Responsibilities |
|------|-----------------|
| **AI Governance Officer** | Overall governance execution, policy enforcement, committee coordination, regulatory compliance |
| **Model Owner** | System performance, fairness, accuracy, documentation, incident reporting |
| **Data Owner** | Training data quality, privacy compliance, bias audits, data retention |
| **Business Sponsor** | Use case definition, stakeholder management, business impact assessment |
| **Technical Lead** | Architecture, development standards, validation procedures, monitoring |
| **Compliance Officer** | Regulatory requirements, audit readiness, legal review, documentation |
| **Data Scientist** | Model development, testing, fairness analysis, performance monitoring |
| **Clinical Lead** (if healthcare) | Clinical validation, safety assessment, medical consensus, human oversight |

### 3.3 Decision Authority

**Who Approves What:**

| Decision | Authority | Timeline |
|----------|-----------|----------|
| New AI system development | AI Governance Committee | Before development starts |
| Production deployment | AI Governance Officer + Business Sponsor | Before go-live |
| High-risk system changes | AI Governance Committee | Before implementation |
| Risk tier or classification change | Compliance Officer + AI Governance Officer | Within 5 business days |
| Incident response | Model Owner + AI Governance Officer | Immediately |
| Policy updates | AI Governance Committee | Quarterly review, changes as needed |

---

## 4. AI System Classification

### 4.1 Classification Framework

All AI systems must be classified using:

**1. NIST AI RMF Impact Categories:**
- **High Impact**: Potential for significant harm to individuals or stakeholders
- **Medium Impact**: Moderate potential for harm or operational disruption
- **Low Impact**: Minimal potential for harm

**2. EU AI Act Risk Tiers** (if EU operations):
- **High-Risk**: Subject to stringent compliance requirements
- **Limited Risk**: Transparency requirements apply
- **Minimal/No Risk**: No specific requirements

**3. Organizational Risk Tier:**
- **Critical**: Business-critical systems; significant financial or reputational risk
- **High**: High-stakes decisions affecting stakeholders; regulatory impact
- **Medium**: Operational systems; moderate impact if failure
- **Low**: Internal productivity tools; minimal external impact

### 4.2 Classification Process

1. **Submit** system for classification via AI Governance Office
2. **Assess** impact, risk factors, and applicable regulations
3. **Determine** NIST + EU AI Act + Organizational tier
4. **Document** classification with rationale
5. **Approve** classification (AI Governance Officer)
6. **Assign** governance requirements per tier

### 4.3 Classification Examples

**Example 1: Customer Recommendation Engine**
- NIST: Medium Impact (affects customer experience)
- EU AI Act: Limited Risk (transparency only)
- Org Tier: Medium
- **Requirements**: Use policy, monitoring, fairness tracking

**Example 2: Credit Lending Decision System**
- NIST: High Impact (affects financial opportunity, fairness)
- EU AI Act: High-Risk (lending decisions)
- Org Tier: Critical
- **Requirements**: Full governance, fairness audits, human oversight, conformity assessment

**Example 3: Clinical Decision Support**
- NIST: High Impact (affects patient safety)
- EU AI Act: High-Risk (clinical decisions)
- Org Tier: Critical
- **Requirements**: Clinical validation, continuous monitoring, fairness audits, incident response

---

## 5. AI Development & Deployment Standards

### 5.1 Development Phase Requirements

**Before Development Begins:**
- [ ] Use case and business case documented
- [ ] Impact assessment completed
- [ ] Risk classification assigned
- [ ] Required governance approvals obtained
- [ ] Data sources identified and assessed
- [ ] Stakeholder consultation completed

**During Development:**
- [ ] Development follows coding and ML standards
- [ ] Data quality checks implemented
- [ ] Bias testing conducted regularly
- [ ] Documentation maintained
- [ ] Version control used
- [ ] Code reviews completed

**Before Deployment:**
- [ ] Validation testing completed
- [ ] Fairness audit conducted and passed
- [ ] Performance metrics established
- [ ] Monitoring systems configured
- [ ] Documentation finalized
- [ ] Approvals obtained from all stakeholders
- [ ] Staff training completed

### 5.2 Data Governance Requirements

**Training Data:**
- [ ] Data sources documented
- [ ] Data quality assessed
- [ ] Bias analysis completed
- [ ] Privacy assessment conducted (DPIA)
- [ ] Consent obtained (where required)
- [ ] Retention and deletion policies defined

**Operational Data:**
- [ ] Input data logged and monitored
- [ ] Data quality checks automated
- [ ] Access controls implemented
- [ ] Encryption applied (in transit and at rest)
- [ ] Audit trails maintained
- [ ] Retention policies enforced

**Sensitive Data** (personal, health, financial):
- [ ] Additional privacy controls applied
- [ ] Regulatory compliance verified (GDPR, HIPAA, etc.)
- [ ] Restricted access controls
- [ ] Enhanced monitoring
- [ ] Regular privacy audits

### 5.3 Model Validation Requirements

All models must undergo:

**Accuracy Testing:**
- [ ] Test on held-out test set separate from training
- [ ] Performance measured on subgroups
- [ ] Edge case and corner case analysis
- [ ] Adversarial robustness testing
- [ ] Performance targets defined and met

**Fairness Testing:**
- [ ] Fairness metrics computed for each protected group
- [ ] Baseline fairness established
- [ ] Bias detection and analysis
- [ ] Disparity ratios calculated
- [ ] Fairness targets defined and validated
- [ ] Mitigation strategies documented

**Safety & Security Testing:**
- [ ] Vulnerability scanning
- [ ] Data privacy testing
- [ ] Model robustness to attacks
- [ ] Failure mode analysis
- [ ] Incident response plan tested

**Business Logic Testing:**
- [ ] Outputs validated against business rules
- [ ] Integration testing with systems
- [ ] Performance and latency testing
- [ ] Scalability assessment
- [ ] Failure and rollback procedures

---

## 6. Monitoring & Performance Management

### 6.1 Monitoring Requirements

**Real-Time Monitoring:**
- [ ] System availability and uptime
- [ ] Latency and performance
- [ ] Input data quality
- [ ] Output anomalies
- [ ] Error rates and exceptions

**Regular Monitoring (Weekly/Monthly):**
- [ ] Accuracy metrics by subgroup
- [ ] Fairness metrics by demographic
- [ ] Data drift detection
- [ ] Performance trends
- [ ] Human override rates
- [ ] System incident logs

**Periodic Monitoring (Quarterly/Annually):**
- [ ] Comprehensive fairness audit
- [ ] Third-party assessment (annual)
- [ ] Stakeholder feedback review
- [ ] Regulatory compliance check
- [ ] Policy and procedure updates

### 6.2 Performance Metrics

**Define for each system:**

| Category | Examples |
|----------|----------|
| **Accuracy** | Precision, Recall, F1-Score, RMSE, AUC-ROC |
| **Fairness** | Demographic parity, equal opportunity, calibration |
| **Safety** | False positive rate, false negative rate, worst-case scenario |
| **Security** | Data breaches, unauthorized access, attack incidents |
| **Performance** | Latency, throughput, availability, resource usage |
| **Business** | Adoption rate, stakeholder satisfaction, ROI |

### 6.3 Alert & Response Thresholds

**Establish thresholds for:**
- Performance degradation (e.g., accuracy drops >5%)
- Fairness metric breach (e.g., disparity ratio >1.25)
- Data drift indicators (e.g., KL divergence >0.05)
- Security or privacy incidents
- System downtime or errors

**Response Protocol:**
1. Alert triggered → Immediate notification
2. Investigation → Within 24 hours
3. Root cause analysis → Within 3-5 business days
4. Corrective action → Within 2-4 weeks (depending on severity)
5. Monitoring enhancement → Within 30 days

---

## 7. Fairness & Bias Management

### 7.1 Fairness Principles

We are committed to:
- **Non-Discrimination**: No discriminatory bias based on protected characteristics
- **Transparency**: Clear understanding of how AI affects decisions
- **Accountability**: Responsibility for fairness outcomes
- **Continuous Improvement**: Regular fairness audits and refinement

### 7.2 Protected Characteristics

Systems must be monitored for fairness across:
- Age
- Gender / Gender Identity
- Race / Ethnicity
- National Origin
- Disability Status
- Religion
- Sexual Orientation
- Veteran Status
- Socioeconomic Status
- [Organization-specific characteristics]

### 7.3 Fairness Audit Procedures

**Monthly Fairness Audit:**
1. Compute fairness metrics for each protected group
2. Compare against baseline and thresholds
3. Identify disparities or concerning patterns
4. Document findings
5. Escalate if thresholds breached

**Quarterly Comprehensive Audit:**
1. Full fairness analysis by all protected characteristics
2. Intersectional analysis (combinations of characteristics)
3. Performance on minority populations
4. Trend analysis (are disparities increasing/decreasing?)
5. Third-party review (if high-risk)
6. Remediation planning for identified disparities

**Remediation Options:**
- Data rebalancing or augmentation
- Model retraining with fairness constraints
- Threshold adjustment
- Monitoring enhancement
- Policy or procedure updates
- System deprovisioning (if unresolvable)

---

## 8. Human Oversight & Explainability

### 8.1 Human-in-the-Loop Requirements

**High-Risk Systems:**
- [ ] Mandatory human review for all decisions
- [ ] Clear escalation procedures
- [ ] Decision override capability
- [ ] Documented reasoning for overrides
- [ ] Regular training for human reviewers

**Medium-Risk Systems:**
- [ ] Human review for borderline or high-confidence predictions
- [ ] Random sampling for quality assurance
- [ ] Exception handling procedures
- [ ] Periodic reviewer training

**Low-Risk Systems:**
- [ ] Spot checking and sampling
- [ ] Feedback mechanisms for user correction
- [ ] Incident-based human review

### 8.2 Explainability Requirements

**High-Risk Systems:**
- [ ] Detailed explanations for each decision
- [ ] Explanation tested for quality and accuracy
- [ ] User-facing explanations in plain language
- [ ] Technical documentation of explanation methods

**Medium-Risk Systems:**
- [ ] Summary explanation of key factors
- [ ] Explanation quality validated
- [ ] Available upon request

**Low-Risk Systems:**
- [ ] General explanation of system purpose
- [ ] Key factors described (may be generic)

### 8.3 Appeals & Remedy Processes

Users or stakeholders affected by AI decisions must have:
- [ ] Right to request human review
- [ ] Appeals process documented
- [ ] Timeline for response (e.g., 30 days)
- [ ] Escalation procedures
- [ ] Remedy options if decision deemed unfair
- [ ] Contact information for appeals

---

## 9. Data Privacy & Security

### 9.1 Privacy Compliance

**GDPR (EU):**
- [ ] Legal basis for processing documented
- [ ] Data Processing Agreement with processors
- [ ] Data retention limits applied
- [ ] Right to access, rectification, erasure procedures
- [ ] Data portability mechanisms
- [ ] Regular Data Protection Impact Assessments

**HIPAA (Healthcare - USA):**
- [ ] Business Associate Agreements with vendors
- [ ] Patient consent procedures
- [ ] Secure data transmission and storage
- [ ] Breach notification procedures
- [ ] Regular HIPAA audits

**CCPA/CPRA (California):**
- [ ] Consumer rights procedures (know, delete, opt-out)
- [ ] Privacy policy requirements
- [ ] Data sale opt-out mechanisms
- [ ] Vendor contracting requirements

**[Other Applicable Regulations]**

### 9.2 Security Controls

**Data Protection:**
- [ ] Encryption in transit (TLS/SSL)
- [ ] Encryption at rest (AES-256 or equivalent)
- [ ] Access controls and authentication
- [ ] Audit logging and monitoring
- [ ] Regular security testing

**Model Protection:**
- [ ] Source code access controls
- [ ] Model artifact encryption
- [ ] Version control and change tracking
- [ ] Deployment authorization procedures
- [ ] Production environment isolation

**Incident Response:**
- [ ] Breach detection procedures
- [ ] Incident response team and protocol
- [ ] Notification procedures (users, regulators)
- [ ] Root cause analysis and remediation
- [ ] Prevention measures for future incidents

---

## 10. Third-Party AI & Vendor Management

### 10.1 Vendor Selection Criteria

When using third-party AI services or models:
- [ ] Vendor governance capabilities assessed
- [ ] Contract terms reviewed (data use, liability, etc.)
- [ ] Security and privacy practices validated
- [ ] Fairness and bias commitments documented
- [ ] Monitoring and audit access confirmed
- [ ] Exit and data return procedures defined

### 10.2 Vendor Contracts

Contracts with AI vendors must include:
- [ ] Data use and protection requirements
- [ ] Performance SLAs and metrics
- [ ] Fairness and bias commitments
- [ ] Security and incident response procedures
- [ ] Audit and monitoring rights
- [ ] Liability and indemnification
- [ ] Data return and destruction on termination
- [ ] Compliance with applicable laws

### 10.3 Ongoing Vendor Management

- [ ] Quarterly vendor performance reviews
- [ ] Annual security and fairness audits
- [ ] Compliance verification
- [ ] Issue escalation procedures
- [ ] Alternative vendor evaluation

---

## 11. Training & Competence

### 11.1 Mandatory Training

**All Staff:**
- [ ] AI governance awareness (annual)
- [ ] Responsible AI principles
- [ ] Bias and fairness basics
- [ ] Data privacy and security

**AI Developers & Data Scientists:**
- [ ] Fairness testing techniques
- [ ] Model validation procedures
- [ ] Bias detection and mitigation
- [ ] Security and privacy in ML
- [ ] Monitoring and drift detection

**Model Owners & Business Leads:**
- [ ] Governance requirements for their systems
- [ ] Performance monitoring and review
- [ ] Incident response procedures
- [ ] Regulatory compliance requirements

**Human Reviewers (for high-risk systems):**
- [ ] System operation and limitations
- [ ] Fairness and bias awareness
- [ ] Decision-making standards
- [ ] Appeal handling

**Compliance & Legal:**
- [ ] AI governance framework
- [ ] Regulatory requirements (NIST, ISO, EU AI Act, etc.)
- [ ] Audit procedures
- [ ] Documentation requirements

### 11.2 Competence Assessment

- [ ] Training completion tracking
- [ ] Knowledge assessments
- [ ] Certification programs (optional)
- [ ] Refresher training (annually)
- [ ] Role-specific competency requirements

---

## 12. Documentation & Record Keeping

### 12.1 Required Documentation

**System-Level Documentation:**
- [ ] Model Card (architecture, performance, limitations)
- [ ] Risk Assessment (NIST AI RMF MAP)
- [ ] Training Data Documentation
- [ ] Fairness Audit Reports
- [ ] Validation & Testing Results
- [ ] Deployment Plan & Procedures
- [ ] Monitoring Plan & Dashboards
- [ ] Incident Reports & Resolutions

**Policy-Level Documentation:**
- [ ] This governance policy
- [ ] System classification decisions
- [ ] Approval records
- [ ] Training completion records
- [ ] Audit reports
- [ ] Third-party assessment results
- [ ] Regulatory correspondence

### 12.2 Record Retention

- **Active Systems**: Maintain documentation for system lifetime + 3-5 years after deprovisioning
- **Audit Trails**: Minimum 5 years for high-risk systems, 2 years for others
- **Training Records**: 3 years
- **Incident Reports**: Minimum 5 years
- **Third-Party Assessments**: 5 years

### 12.3 Documentation Location & Access

- [ ] Central documentation repository established
- [ ] Version control implemented
- [ ] Access controls configured (read/write/delete)
- [ ] Regular backups taken
- [ ] Search and retrieval capabilities
- [ ] Archive procedures for inactive systems

---

## 13. Incident Management

### 13.1 Incident Definition & Reporting

**AI System Incidents include:**
- Performance degradation or accuracy drop
- Fairness metric breach or detected bias
- Data privacy or security incident
- Unauthorized access or misuse
- System failure or availability issue
- Stakeholder complaint or harm report
- Regulatory inquiry or enforcement action

**Reporting Requirements:**
- [ ] Incidents reported to AI Governance Officer within 24 hours
- [ ] High-priority incidents reported immediately
- [ ] Detailed incident report within 3-5 business days
- [ ] Root cause analysis within 2 weeks
- [ ] Corrective action plan within 30 days

### 13.2 Incident Response Team

**Team Members:**
- AI Governance Officer (Chair)
- Model Owner
- Data Owner
- Compliance Officer (if regulatory impact)
- Legal Counsel (if needed)
- Chief Medical Officer (if clinical impact)
- Chief Security Officer (if security impact)

**Responsibilities:**
- [ ] Immediate system assessment
- [ ] Stakeholder notification (if required)
- [ ] Investigation and root cause analysis
- [ ] Corrective action implementation
- [ ] Prevention of recurrence
- [ ] Regulatory reporting (if required)
- [ ] Documentation and learning

### 13.3 Escalation Procedures

| Severity | Timeline | Authority | Actions |
|----------|----------|-----------|---------|
| **Critical** | Immediate | CEO / Board | System shutdown if necessary, immediate notifications |
| **High** | 4 hours | AI Governance Committee | Investigation, corrective action, monitoring |
| **Medium** | 24 hours | AI Governance Officer | Investigation, remediation plan |
| **Low** | 5 days | Model Owner | Investigation, monitoring |

---

## 14. Continuous Improvement

### 14.1 Review & Update Cycle

**Quarterly Review:**
- [ ] Policy effectiveness assessment
- [ ] Emerging risks or issues identification
- [ ] Staff feedback collection
- [ ] Framework update tracking (NIST, ISO, EU AI Act changes)

**Annual Comprehensive Review:**
- [ ] Full policy refresh
- [ ] Stakeholder consultation
- [ ] Regulatory compliance assessment
- [ ] Governance maturity evaluation
- [ ] Policy updates and approval

### 14.2 Improvement Triggers

Review policy immediately if:
- Major incident occurs
- Regulatory guidance changes
- Framework standards updated
- Significant organizational change
- Stakeholder complaints
- Third-party audit findings

### 14.3 Feedback Mechanisms

- Staff suggestion process (ideas for improvements)
- Stakeholder feedback (customers, patients, employees)
- Audit findings (internal and external)
- Incident learnings
- Regulatory developments

---

## 15. Governance Reporting

### 15.1 Internal Reporting

**Monthly Reports** (to AI Governance Officer):
- System performance metrics
- Fairness audit results
- Incident summary
- Training completion
- Emerging issues

**Quarterly Reports** (to AI Governance Committee):
- Portfolio overview (all systems status)
- Risk summary (high-risk systems performance)
- Incident analysis (patterns, trends)
- Compliance status
- Recommendations for approval/action

**Annual Reports** (to Board/Executives):
- Strategic AI governance assessment
- Key achievements and improvements
- Risk landscape
- Regulatory compliance status
- Budget and resource needs
- Roadmap for next year

### 15.2 External Reporting

**Regulatory Reports** (as required):
- EU AI Act conformity assessments (for high-risk systems)
- GDPR Data Protection Impact Assessments
- HIPAA Breach notifications
- Fair lending audits
- [Other regulatory requirements]

**Transparency Reports** (optional, recommended):
- AI system inventory (public-facing)
- Performance and fairness metrics
- Known limitations and risks
- Human oversight and appeal procedures
- Contact information for inquiries

---

## 16. Compliance & Enforcement

### 16.1 Compliance Expectations

All staff must:
- [ ] Understand applicable governance policies
- [ ] Comply with classification and approval procedures
- [ ] Participate in required training
- [ ] Support monitoring and auditing
- [ ] Report incidents and concerns
- [ ] Document decisions and actions
- [ ] Maintain confidentiality of sensitive information

### 16.2 Audit & Assurance

**Internal Audits:**
- [ ] Quarterly audits of selected systems
- [ ] Annual comprehensive governance audit
- [ ] Risk-based audit scheduling
- [ ] Findings and remediation tracking

**External Audits:**
- [ ] Annual third-party assessment (for high-risk systems)
- [ ] Regulatory audits (as required)
- [ ] Assessment results documented
- [ ] Remediation for findings

### 16.3 Violations & Enforcement

**Minor Violations** (e.g., missed training):
- Reminder and corrective action plan
- Supervisor notification
- Monitoring of compliance

**Moderate Violations** (e.g., governance procedure not followed):
- Formal notice
- Corrective action plan
- Performance evaluation impact

**Serious Violations** (e.g., deploying high-risk system without approval):
- Formal investigation
- System deployment halt
- Disciplinary action up to termination
- Regulatory notification (if required)

---

## 17. Policy Governance

### 17.1 Policy Authority & Approval

**Policy Owner**: [Chief Risk Officer / AI Governance Officer]  
**Approval Authority**: [Board / Executive Committee / CEO]  
**Review Cycle**: Annually or as needed

### 17.2 Policy Changes

**Process for Policy Updates:**
1. Proposed change submitted to Policy Owner
2. Impact assessment conducted
3. Stakeholder consultation
4. Draft updated policy
5. Legal and compliance review
6. Approval authority review and approval
7. Staff notification and training
8. Implementation and monitoring

### 17.3 Policy Exceptions

**Exception Request Process:**
- Submit exception request with business justification
- AI Governance Committee review
- Risk assessment of exception
- Approval or denial
- Monitoring if approved
- Expiration date set

---

## 18. Attachments & References

### Attachment A: Acronyms & Abbreviations
- AI: Artificial Intelligence
- ML: Machine Learning
- NIST: National Institute of Standards and Technology
- RMF: Risk Management Framework
- ISO: International Organization for Standardization
- EU: European Union
- GDPR: General Data Protection Regulation
- HIPAA: Health Insurance Portability and Accountability Act
- CCPA: California Consumer Privacy Act
- [Others as applicable]

### Attachment B: Related Policies & Documents
- Data Privacy Policy
- Information Security Policy
- Data Governance Policy
- Code of Conduct
- Vendor Management Policy
- [Organization-specific policies]

### Attachment C: External Frameworks & Standards
- NIST AI Risk Management Framework: https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf
- ISO/IEC 42001:2023: https://www.iso.org/standard/81230.html
- EU AI Act: https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:32024R1689
- GDPR: https://gdpr-info.eu/
- HIPAA: https://www.hhs.gov/hipaa/
- CCPA: https://oag.ca.gov/privacy/ccpa

### Attachment D: Governance Contacts
- AI Governance Officer: [Name, email, phone]
- Chief Risk Officer: [Name, email, phone]
- Compliance Officer: [Name, email, phone]
- Data Privacy Officer: [Name, email, phone]
- Chief Information Security Officer: [Name, email, phone]

---

## 19. Approval Sign-Off

**Policy Approvals:**

- [ ] Policy Owner: _________________________ Date: _______
  
- [ ] General Counsel: _________________________ Date: _______
  
- [ ] Chief Risk Officer: _________________________ Date: _______
  
- [ ] Board/Executive Committee: _________________________ Date: _______

**Effective Date:** [Date when policy takes effect]

---

**Document Version**: 1.0  
**Last Updated**: September 2026  
**Next Review**: [Date]  
**Classification**: Internal / Confidential

---

## Document Control

| Version | Date | Changes | Author |
|---------|------|---------|--------|
| 1.0 | 2026-09-10 | Initial policy | [Name] |
| | | | |
| | | | |

---

**Questions or Feedback?**  
Contact: [AI Governance Officer Email]
