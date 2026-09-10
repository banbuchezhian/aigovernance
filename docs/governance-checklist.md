# AI Governance Implementation Checklist

Use this checklist to implement AI governance across NIST AI RMF, ISO/IEC 42001, and EU AI Act frameworks.

---

## Phase 1: Prepare & Classify

### 1.1 Governance Structure (ISO 42001 / NIST GOVERN)
- [ ] AI governance model defined (e.g., AI Governance Committee structure)
- [ ] Roles and responsibilities documented (AI Owner, Data Owner, Model Owner, etc.)
- [ ] Decision authority and escalation paths established
- [ ] Stakeholder identification completed (internal and external)
- [ ] Governance committee charter approved
- [ ] Communication and reporting cadence established

### 1.2 AI System Inventory (ISO 42001 / NIST MAP)
- [ ] All AI systems cataloged in central registry
- [ ] System descriptions and use cases documented
- [ ] Stakeholder identification per system
- [ ] Intended and foreseeable misuse scenarios identified
- [ ] Data sources and data flows mapped
- [ ] Dependencies on third-party AI services documented

### 1.3 Risk Classification (NIST MAP / EU AI Act)
- [ ] NIST AI RMF impact assessment completed
  - [ ] Impact type identified (mission, economic, civil rights, etc.)
  - [ ] Severity and likelihood estimated
  - [ ] Stakeholder impact analyzed
- [ ] EU AI Act risk tier determined
  - [ ] Prohibited risk assessment completed
  - [ ] High-risk criteria evaluation documented
  - [ ] Classification rationale documented
- [ ] Classification approved by governance authority

### 1.4 Governance Planning (ISO 42001)
- [ ] Governance roadmap created
- [ ] Required policies and procedures identified
- [ ] Resource requirements and budget estimated
- [ ] Timeline for implementation established
- [ ] Stakeholder communication plan developed
- [ ] Training needs identified

---

## Phase 2: Establish Governance Framework

### 2.1 Policy & Governance Documents (ISO 42001)
- [ ] AI Governance Policy drafted and approved
- [ ] Risk Management Policy specific to AI documented
- [ ] Data Governance Policy for AI training/operational data created
- [ ] Model Management Policy established
- [ ] Fairness & Bias Policy documented
- [ ] Explainability & Transparency Policy defined
- [ ] Incident Response Policy for AI systems created
- [ ] Third-Party AI Services Policy (if applicable) established

### 2.2 NIST AI RMF Documentation (NIST)
For each system, document:
- [ ] **MAP Phase**
  - [ ] System context and stakeholders
  - [ ] AI lifecycle and data flows
  - [ ] Risk categorization (impact, performance, security, fairness)
  - [ ] Measurement approach defined
- [ ] **MEASURE Phase**
  - [ ] Performance metrics and thresholds defined
  - [ ] Fairness metrics and baselines established
  - [ ] Security metrics defined
  - [ ] Data quality metrics identified
  - [ ] Monitoring plan created
- [ ] **MANAGE Phase**
  - [ ] Risk mitigation controls identified
  - [ ] Control implementation plan created
  - [ ] Responsibility assignments documented
- [ ] **GOVERN Phase**
  - [ ] Governance processes integrated
  - [ ] Review and improvement cadence set
  - [ ] Stakeholder communication plan established

### 2.3 EU AI Act Compliance Plan (EU AI Act)
For High-Risk systems, prepare:
- [ ] Risk tier classification documented with rationale
- [ ] Conformity assessment plan established
- [ ] Technical documentation outline created
- [ ] Audit trail logging requirements defined
- [ ] Transparency requirements identified
- [ ] Human oversight procedures documented
- [ ] Quality assurance procedures planned

### 2.4 Data Governance (NIST MEASURE / ISO 42001)
- [ ] Training data inventory created
- [ ] Data source documentation completed
- [ ] Data quality assessment conducted
- [ ] Data bias audit plan established
- [ ] Data retention and deletion policies defined
- [ ] Data access control procedures implemented
- [ ] Sensitive data protection measures identified

---

## Phase 3: Implement Controls & Monitoring

### 3.1 Model Development & Validation (ISO 42001 / NIST MEASURE)
- [ ] Model development standards established
- [ ] Data collection and preparation procedures documented
- [ ] Feature engineering approach documented
- [ ] Model selection and training procedures created
- [ ] Model validation plan established:
  - [ ] Accuracy testing on held-out test sets
  - [ ] Fairness testing across demographic groups
  - [ ] Adversarial robustness testing
  - [ ] Edge case and corner case analysis
  - [ ] Performance on minority populations
- [ ] Model card created with:
  - [ ] Architecture and training approach
  - [ ] Performance metrics (overall and disaggregated)
  - [ ] Training data description
  - [ ] Known limitations and bias
  - [ ] Recommended use cases and constraints
- [ ] Model documentation approved by governance

### 3.2 Fairness & Bias Controls (NIST MANAGE / ISO 42001)
- [ ] Fairness metrics defined for each protected characteristic
- [ ] Baseline fairness measurements established
- [ ] Bias detection procedures implemented
- [ ] Bias mitigation strategies documented:
  - [ ] Pre-processing: data balancing, synthetic data, etc.
  - [ ] In-processing: fairness-aware algorithms, constraints
  - [ ] Post-processing: threshold adjustment, outcome adjustment
- [ ] Fairness testing automated in CI/CD pipeline
- [ ] Regular fairness audit schedule established
- [ ] Bias monitoring dashboard created
- [ ] Escalation procedures for bias breaches documented

### 3.3 Explainability & Transparency (NIST MEASURE / EU AI Act)
- [ ] Explainability requirements defined (by risk tier/use case)
- [ ] Explainability methods selected:
  - [ ] Feature importance (SHAP, LIME, etc.)
  - [ ] Decision rules or logic explanations
  - [ ] Saliency maps or attention visualizations
  - [ ] Counterfactual explanations
- [ ] Explanation quality metrics established and measured
- [ ] User-facing transparency mechanisms implemented
- [ ] Explanation validation with stakeholders completed
- [ ] Documentation of explanations and limitations prepared

### 3.4 Human Oversight & Review (NIST MANAGE / EU AI Act)
- [ ] Human review procedures documented
- [ ] Decision thresholds for human review established
- [ ] Escalation procedures for model disagreements created
- [ ] Human reviewer training program developed
- [ ] Override tracking and logging implemented
- [ ] Appeal and dispute resolution process documented
- [ ] Human review SLAs established
- [ ] Human reviewer performance metrics defined

### 3.5 Monitoring & Performance Tracking (NIST MEASURE / ISO 42001)
- [ ] Monitoring dashboard created with:
  - [ ] Real-time performance metrics
  - [ ] Fairness metric tracking
  - [ ] Data quality metrics
  - [ ] System availability and latency
  - [ ] Human override rates
  - [ ] Alert thresholds and notifications
- [ ] Monitoring frequency established (real-time / daily / weekly / etc.)
- [ ] Performance SLAs defined
- [ ] Drift detection mechanisms implemented
- [ ] Anomaly detection alerts configured
- [ ] Monitoring logs automated and retained
- [ ] Alert response procedures documented

### 3.6 Security & Data Protection (NIST MEASURE / ISO 42001)
- [ ] Data encryption implemented (in transit and at rest)
- [ ] Access control procedures implemented
- [ ] Authentication and authorization mechanisms in place
- [ ] Model artifact protection measures taken
- [ ] Adversarial attack testing conducted
- [ ] Security incident procedures documented
- [ ] Regular penetration testing scheduled
- [ ] Privacy impact assessment (DPIA) completed

---

## Phase 4: Audit, Review & Continuous Improvement

### 4.1 Internal Audit Program (ISO 42001)
- [ ] Internal audit schedule established (quarterly minimum)
- [ ] Audit checklist developed
- [ ] Audit procedures documented
- [ ] Audit evidence collection methods defined
- [ ] Audit findings and remediation process established
- [ ] Audit report template created
- [ ] Audit results trending tracked

### 4.2 Quarterly System Reviews (NIST GOVERN / ISO 42001)
- [ ] Review cadence established (quarterly recommended)
- [ ] Review participants defined (model owner, data owner, governance officer, etc.)
- [ ] Review agenda items:
  - [ ] Performance vs. SLAs
  - [ ] Fairness metrics vs. baselines
  - [ ] Incident review (if any)
  - [ ] Drift and monitoring results
  - [ ] Change requests and versioning
  - [ ] Stakeholder feedback
- [ ] Review meeting minutes documented
- [ ] Action items tracked and resolved

### 4.3 Annual Third-Party Assessment (ISO 42001 / EU AI Act)
- [ ] Independent assessor identified (for High-Risk systems)
- [ ] Assessment scope and criteria defined
- [ ] Assessment timeline established
- [ ] Assessment checklist/criteria provided to assessor
- [ ] Assessment conducted and findings documented
- [ ] Remediation plan for any findings created
- [ ] Assessment report retained for compliance

### 4.4 Model Retraining & Versioning (ISO 42001 / NIST MANAGE)
- [ ] Retraining triggers defined:
  - [ ] Performance degradation threshold
  - [ ] Drift detection
  - [ ] Data distribution change
  - [ ] Fairness metric breach
  - [ ] Scheduled retraining (e.g., quarterly)
- [ ] Retraining procedure documented
- [ ] Model versioning scheme established
- [ ] Rollback procedures defined
- [ ] Retraining validation requirements documented
- [ ] Change log maintained for all model versions

### 4.5 Continuous Improvement (ISO 42001)
- [ ] Improvement opportunities tracking system established
- [ ] Improvement backlog prioritization process defined
- [ ] Lessons learned documentation process created
- [ ] Feedback mechanisms from stakeholders implemented
- [ ] Annual governance program review scheduled
- [ ] Framework updates tracked (NIST, ISO, EU AI Act changes)
- [ ] Policy updates process established

### 4.6 Incident Management (ISO 42001 / NIST MANAGE)
- [ ] Incident definition and severity levels documented
- [ ] Incident reporting channels established
- [ ] Incident investigation procedures created
- [ ] Root cause analysis process documented
- [ ] Corrective action implementation tracking system
- [ ] Incident communication and notification procedure defined
- [ ] Incident log maintained and analyzed for patterns
- [ ] Post-incident reviews scheduled

---

## Phase 5: Documentation & Evidence

### 5.1 Governance Documentation Repository (ISO 42001)
- [ ] Central documentation repository established
- [ ] Version control implemented
- [ ] Access control configured
- [ ] Documentation review and approval process created
- [ ] Documentation retention policy defined
- [ ] Search and retrieval procedures documented

### 5.2 Compliance Evidence Retention (EU AI Act)
For High-Risk systems, retain:
- [ ] Risk assessment reports
- [ ] Training data documentation
- [ ] Testing and validation reports
- [ ] Audit trails and logs
- [ ] Conformity assessment reports
- [ ] Incident reports
- [ ] Monitoring reports and metrics
- [ ] Third-party assessment reports

### 5.3 Audit Trail & Logging (EU AI Act / NIST)
- [ ] Logging requirements defined
- [ ] Logging mechanism implemented:
  - [ ] Input data logged (with privacy protections)
  - [ ] Model decisions and confidence scores logged
  - [ ] Human reviews and overrides logged
  - [ ] System changes logged
- [ ] Log retention policy defined (typically 3-5 years minimum)
- [ ] Log access control and integrity measures
- [ ] Log analysis procedures for anomaly detection
- [ ] Log export capabilities for auditors

### 5.4 Transparency & Public Reporting (EU AI Act optional, best practice)
- [ ] AI system use disclosure procedure
- [ ] Transparency report template created
- [ ] System performance metrics published (where appropriate)
- [ ] Known limitations and risks disclosed
- [ ] Third-party assessment results shared (if not confidential)
- [ ] Contact information for inquiries provided

---

## Phase 6: Ongoing Governance

### 6.1 Governance Maturity Assessment
- [ ] Initial maturity level assessed
- [ ] Maturity improvement roadmap created
- [ ] Target maturity level defined
- [ ] Progress tracking established

### 6.2 Training & Competence (ISO 42001)
- [ ] Governance awareness training conducted
- [ ] Role-specific training developed:
  - [ ] Model developers on fairness and bias
  - [ ] Data engineers on data quality
  - [ ] Operational staff on incident response
  - [ ] Leadership on governance oversight
- [ ] Competence assessment conducted
- [ ] Training records maintained

### 6.3 Stakeholder Engagement (NIST GOVERN)
- [ ] Stakeholder feedback mechanisms implemented
- [ ] Regular stakeholder communication established
- [ ] Advisory groups or councils formed (if appropriate)
- [ ] External accountability mechanisms (if applicable)

### 6.4 Regulatory & Framework Evolution
- [ ] Monitoring process for regulatory changes established
- [ ] NIST AI RMF updates tracked
- [ ] ISO/IEC 42001 updates tracked
- [ ] EU AI Act implementation guidance followed
- [ ] Quarterly governance program review conducted
- [ ] Framework compliance assessment updated annually

---

## Checklist Scoring

Use this checklist to assess governance maturity:

**Maturity Levels:**
- **Level 1 (Ad Hoc)**: <25% items completed
- **Level 2 (Developing)**: 25-50% items completed
- **Level 3 (Implemented)**: 50-75% items completed
- **Level 4 (Optimized)**: 75-100% items completed

**Scoring by Phase:**
- Phase 1: ___/24 (Prepare & Classify)
- Phase 2: ___/30 (Establish Framework)
- Phase 3: ___/45 (Implement Controls)
- Phase 4: ___/30 (Audit & Review)
- Phase 5: ___/20 (Documentation)
- Phase 6: ___/15 (Ongoing)

**Total: ___/164**

---

## Usage Tips

1. **For New Programs**: Complete sequentially through all phases
2. **For Existing Programs**: Start with Phase 1 assessment, then fill gaps
3. **For Risk-Tier-Based Implementation**: Prioritize high-risk systems
4. **For Audit Preparation**: Focus on documentation and evidence gathering phases
5. **For Continuous Improvement**: Review quarterly and update roadmap

---

**Last Updated**: September 2026  
**Compatible With**: NIST AI RMF 1.0 | ISO/IEC 42001:2023 | EU AI Act (2024/1689)
