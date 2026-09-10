# Scenario: MedSecure Health Applies the Framework Lens

## Company Overview
**Organization:** MedSecure Health  
**Industry:** Healthcare  
**Region:** USA + EU  
**Compliance Requirements:** HIPAA + GDPR + EU AI Act (High-Risk Classification)

---

## AI Projects

### Project A: Staff Copilot
Approved public GenAI tool for internal productivity, drafting, summarization, and policy Q&A. Helps staff members write communications, summarize documents, and answer organizational policy questions.

**Key Features:**
- Internal productivity assistance only
- No training on patient or confidential data
- Helps with documentation and communication
- Policy and best practices guidance

**Governance Focus:** Data boundaries, acceptable use, staff training

---

### Project B: Clinical Decision Agent
Custom agentic AI system using RAG and clinical data to support clinicians with patient history, evidence-based treatment summaries, and decision support for diagnosis and treatment recommendations.

**Key Features:**
- Patient history summarization
- Clinical evidence integration
- Treatment recommendation support
- Human-in-the-loop clinical review
- HIPAA-compliant data handling

**Governance Focus:** Clinical safety, accuracy validation, bias detection, human oversight

---

## Framework Mapping

### How It Helps MedSecure Ask the Right Questions

| Framework | What It Helps MedSecure Ask | Staff Copilot | Clinical Decision Agent |
|-----------|---------------------------|---------------|------------------------|
| **NIST AI RMF** | Have we governed, measured, and managed AI risk? | Map users, data restrictions, vendor risk, and acceptable use. | Map clinical context, patient impact, performance, safety, drift, and residual risk. |
| **ISO/IEC 42001** | Is AI governance structured, resourced, documented, measured, and improved? | Define policy, training, records, owners, and review cadence. | Establish formal AIMS controls, lifecycle ownership, clinical review procedures, and continuous monitoring. |
| **EU AI Act** | What risk tier, role, and evidence obligations apply? | Limited risk if scoped to productivity with no sensitive decisions. Likely no high-risk if no patient data processed. | Classified as High-Risk (clinical decision support affecting patient treatment). Requires conformity assessment, technical documentation, clinical validation, and ongoing monitoring. |

---

## Governance Implementation

### NIST AI RMF: MAP Phase
**What to Document:**

**Staff Copilot:**
- User groups: Administrative staff, clinical support, documentation teams
- Data restrictions: No patient data, no confidential medical information
- Vendor risk: Third-party GenAI provider, data use agreements
- Stakeholder impact: Staff productivity, documentation quality
- Acceptable use: Approved use cases and prohibited uses

**Clinical Decision Agent:**
- Clinical context: Emergency department triage, inpatient diagnosis support
- Patient impact: Treatment recommendations affect clinical decisions
- Clinical users: Physicians, nurses, clinical staff
- Data sources: EHR, lab results, imaging reports, patient history
- Stakeholder impact: Patient safety, care quality, clinician workflow

---

### NIST AI RMF: MEASURE Phase
**What to Track:**

**Staff Copilot:**
- Output quality: Usefulness scores from staff feedback
- Safety: Misuse incidents, policy violations
- Data security: No unauthorized data access
- Fairness: Equal quality across user types and departments

**Clinical Decision Agent:**
- Clinical accuracy: Recommendation alignment with final clinical diagnosis
- Safety metrics: Adverse events, missed diagnoses, wrong treatment suggestions
- Bias metrics: Recommendation quality across patient demographics (age, gender, race, socioeconomic status)
- Performance: Latency, availability, uptime
- Human oversight: Override rates, disagreement tracking
- Drift detection: Performance degradation triggers for retraining

---

### ISO/IEC 42001: Governance Structure

**Staff Copilot Governance:**
- **Policy:** GenAI acceptable use policy for staff productivity
- **Ownership:** IT Director + Compliance Officer
- **Training:** Mandatory staff training on acceptable use and data protection
- **Review Cadence:** Quarterly incident review, annual policy refresh
- **Documentation:** Use case inventory, incident logs, training records

**Clinical Decision Agent Governance:**
- **Policy:** Clinical AI governance policy covering clinical decision support systems
- **Ownership:** Chief Medical Officer + AI Governance Officer
- **AIMS Controls:**
  - Model lifecycle management (development, validation, deployment, monitoring)
  - Clinical validation procedures
  - Fairness testing protocols
  - Performance monitoring dashboards
  - Incident response procedures
- **Review Cadence:** Monthly clinical review, quarterly fairness audit, annual external assessment
- **Documentation:** Clinical validation reports, fairness audit results, incident logs

---

### EU AI Act: Compliance Requirements

**Staff Copilot Classification:**
- **Risk Tier:** Limited Risk (if scoped to productivity with no sensitive decisions)
- **Requirements:**
  - Transparency: Users informed AI is assisting with drafting
  - Acceptable use policy documented
  - Data use agreement with vendor
  - No special obligations if truly non-high-risk

**Clinical Decision Agent Classification:**
- **Risk Tier:** High-Risk (clinical decision support affects patient treatment)
- **Conformity Assessment Required:**
  - Technical documentation of system and algorithms
  - Training data documentation and validation
  - Clinical validation evidence
  - Performance testing across populations
  - Fairness and bias assessment
  - Human oversight procedures
  - Monitoring plan
- **Documentation Requirements:**
  - Model card and system specifications
  - Clinical validation report
  - Fairness audit report
  - Risk assessment and mitigation plan
  - User manual and clinical guidelines
  - Incident response procedures
  - Audit trail logging specifications
- **Ongoing Obligations:**
  - Continuous performance monitoring
  - Quarterly fairness reviews
  - Annual third-party assessment
  - Audit trail maintenance (minimum 3-5 years)
  - Post-market surveillance for adverse events

---

## Key Governance Artifacts

### For Staff Copilot
1. **GenAI Acceptable Use Policy** - When and how staff can use the tool
2. **Data Handling Agreement** - Vendor data use terms and restrictions
3. **Training Program** - Mandatory staff education on responsible use
4. **Incident Log** - Track any policy violations or misuse
5. **Quarterly Review Report** - Summary of usage patterns and incidents

### For Clinical Decision Agent
1. **Clinical Validation Report** - Evidence that recommendations are clinically sound
2. **Model Card** - Architecture, training data, performance metrics, limitations
3. **Data Privacy Impact Assessment** - HIPAA and GDPR compliance validation
4. **Fairness Audit Report** - Bias testing across patient demographics
5. **Human Review Protocol** - Decision review thresholds and escalation procedures
6. **Conformity Assessment Report** - EU AI Act compliance documentation
7. **Risk Management Plan** - Monitoring, incident response, drift detection
8. **Audit Trail Specifications** - What decisions to log and how long to retain
9. **Third-Party Assessment** - Annual independent clinical validation

---

## Clinical Safety & Governance Focus

### Risk Assessment

**Clinical Decision Agent High-Risk Areas:**

1. **Patient Safety Risk**
   - Wrong diagnosis recommendations → missed or incorrect treatment
   - Bias in recommendations by patient demographics → unequal care quality
   - Performance degradation over time → outdated recommendations

2. **Data Privacy Risk**
   - Patient data handling (HIPAA compliance)
   - EU patient data (GDPR compliance)
   - Audit trail security and retention

3. **Clinical Validity Risk**
   - Model performance on diverse patient populations
   - Validation against latest clinical guidelines
   - Handling of rare or complex cases

### Mitigation Strategies

**Clinical Governance Controls:**
- [ ] Clinical validation team (physicians) reviews all recommendations
- [ ] Human override required for all treatment recommendations
- [ ] Mandatory human review for borderline cases
- [ ] Weekly clinical oversight meeting
- [ ] Monthly fairness audit across patient demographics
- [ ] Quarterly retraining when performance drifts

**Data Governance Controls:**
- [ ] HIPAA-compliant data handling procedures
- [ ] GDPR Data Processing Agreement with vendors
- [ ] Encryption of patient data in transit and at rest
- [ ] Access controls limiting data exposure
- [ ] Audit logging of all data access
- [ ] Data retention policies (minimum 5 years for regulatory, then deletion)

**Performance Governance Controls:**
- [ ] Real-time performance monitoring dashboard
- [ ] Accuracy tracking by patient demographics
- [ ] Fairness metric thresholds and alerts
- [ ] Automated drift detection
- [ ] Retraining triggers when thresholds breached

---

## Fairness & Bias Considerations

### Fairness Metrics to Track

**Clinical Decision Agent Fairness:**

| Metric | Threshold | Monitoring |
|--------|-----------|-----------|
| **Demographic Parity** | <5% difference in recommendation rate across groups | Weekly |
| **Equal Opportunity** | <5% difference in true positive rate across demographics | Weekly |
| **Calibration** | Confidence scores accurate within ±2% across groups | Monthly |
| **Adverse Impact** | No protected group receives <80% of majority recommendation rate | Monthly |

### Protected Groups to Monitor
- Age groups (pediatric, adult, geriatric)
- Gender identity
- Race and ethnicity
- Socioeconomic status
- Insurance type
- Language/literacy

### Fairness Response Plan
- [ ] Monthly fairness audit completed
- [ ] If threshold breached: escalate to Chief Medical Officer within 24 hours
- [ ] Investigation: understand root cause (data bias? model bias? clinical reality?)
- [ ] Remediation: retrain, adjust, or update clinical guidelines as needed
- [ ] Communication: inform clinical staff of any issues and mitigations

---

## Human Oversight & Clinical Review

### Decision Review Protocol

**For Staff Copilot:**
- Staff review all AI-generated content before sending
- Flag any inaccurate or inappropriate suggestions
- Manual review process (no automated approval)

**For Clinical Decision Agent:**
- [ ] All recommendations require physician review
- [ ] Thresholds for mandatory review:
  - High-risk diagnoses (cancer, cardiac, neurologic): 100% review
  - Moderate-risk recommendations: 50% random review
  - Low-risk supportive recommendations: 10% spot check
- [ ] Override tracking: log when clinician disagrees with recommendation
- [ ] Appeal process: patients can request second opinion
- [ ] Feedback loop: clinicians document outcomes to improve future recommendations

### Escalation Procedures
1. Clinician disagrees with high-risk recommendation → Immediate escalation to attending physician
2. Recommendation linked to adverse outcome → Clinical incident review within 24 hours
3. Pattern of bias detected → Chief Medical Officer involvement, system evaluation
4. System unavailability → Manual clinical workflow procedures activate

---

## Monitoring & Continuous Improvement

### Real-Time Monitoring Dashboard

**Staff Copilot Metrics:**
- Daily active users
- Most common use cases
- Customer feedback score
- Policy violation incidents
- Data security events

**Clinical Decision Agent Metrics:**
- Clinical recommendations per day
- Physician override rate (target: <10%)
- System availability and latency
- Patient outcomes tracking
- Fairness metrics (demographic breakdowns)
- Adverse event reports
- Model drift indicators

### Review Cadence

| Frequency | Review Type | Participants | Actions |
|-----------|------------|--------------|---------|
| **Weekly** | Fairness metrics | AI team, Clinical staff | Check thresholds, identify anomalies |
| **Monthly** | Clinical performance | Chief Medical Officer, Clinicians | Validate accuracy, outcomes, bias |
| **Quarterly** | Comprehensive audit | External auditors, Compliance | Full fairness audit, safety assessment |
| **Annually** | Strategic review | Board, Leadership | Outcomes, improvements, renewal decisions |

### Incident Response

**For any adverse event:**
1. Immediate escalation to Chief Medical Officer
2. Investigation: What happened? Was AI involved? Did it contribute?
3. Documentation: Incident report with findings
4. Mitigation: Fix identified issues (retrain model, update guidelines, etc.)
5. Communication: Inform affected patients and clinicians
6. Prevention: Process changes to prevent recurrence
7. Reporting: Regulatory reporting if required by law

---

## Compliance Evidence & Documentation

### HIPAA Compliance
- [ ] Business Associate Agreements with vendors
- [ ] Data encryption in transit and at rest
- [ ] Access controls and audit logs
- [ ] Breach notification procedures
- [ ] Patient privacy training for staff
- [ ] Regular HIPAA security audits

### GDPR Compliance (for EU patients)
- [ ] Data Processing Agreements with vendors
- [ ] Legal basis for processing documented (e.g., healthcare necessity)
- [ ] Patient rights procedures (access, rectification, erasure, portability)
- [ ] Automated decision-making notifications
- [ ] Data retention policies and deletion procedures
- [ ] Data Protection Impact Assessment (DPIA)
- [ ] Consent management where required

### EU AI Act Compliance (High-Risk)
- [ ] Risk assessment documentation
- [ ] Technical documentation and model card
- [ ] Clinical validation evidence
- [ ] Fairness audit reports
- [ ] Human oversight procedures documented
- [ ] Monitoring and performance tracking plan
- [ ] Conformity assessment report
- [ ] Audit trail logging specifications
- [ ] Post-market surveillance procedures

---

## Governance Roadmap

### Phase 1: Foundation (Months 1-2)
- [ ] Governance policies approved (Staff Copilot and Clinical Agent)
- [ ] Roles and responsibilities assigned
- [ ] Compliance framework selected (NIST + ISO + EU AI Act)
- [ ] Risk assessments completed

### Phase 2: Implementation (Months 3-4)
- [ ] Clinical validation completed for Clinical Agent
- [ ] Fairness baselines established and monitored
- [ ] Human review procedures implemented
- [ ] Monitoring dashboards deployed
- [ ] Staff and clinician training completed

### Phase 3: Monitoring (Months 5-6)
- [ ] Real-time monitoring operational
- [ ] Monthly clinical reviews running
- [ ] Fairness audits executed on schedule
- [ ] Incident response procedures tested
- [ ] Documentation for compliance audit prepared

### Phase 4: Optimization (Ongoing)
- [ ] Continuous fairness monitoring
- [ ] Model retraining as needed
- [ ] Clinical guideline updates
- [ ] Staff feedback incorporated
- [ ] Annual third-party assessments

---

## Key Success Metrics

**Staff Copilot:**
- Staff productivity improvement: 15-20% reduction in documentation time
- Staff satisfaction: >80% find tool helpful
- Incident rate: <1 policy violation per 100 users per month
- Data security: 0 unauthorized data access events

**Clinical Decision Agent:**
- Clinical accuracy: >95% alignment with final diagnosis for tested cases
- Safety: <1 adverse event per 10,000 recommendations
- Fairness: <2% performance variance across patient demographics
- Adoption: >70% of clinicians using for eligible cases
- Physician override: 5-10% (appropriate skepticism)

---

## Conclusion

MedSecure Health demonstrates how to apply all three frameworks (NIST AI RMF, ISO/IEC 42001, EU AI Act) to healthcare AI systems at different risk levels:

- **Staff Copilot**: Limited risk, straightforward governance with use policy and training
- **Clinical Decision Agent**: High-risk, comprehensive governance with clinical validation, fairness audits, and ongoing monitoring

Both systems require strong governance infrastructure, human oversight, continuous monitoring, and commitment to fairness and safety as core values.

---

**Template Version**: 1.0  
**Last Updated**: September 2026  
**Compatible With**: NIST AI RMF 1.0 | ISO/IEC 42001:2023 | EU AI Act (2024/1689)
