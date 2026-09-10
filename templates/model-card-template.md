# Model Card Template

Use this template to document all AI models in your organization. Maintain one model card per model/version.

---

## Model Information

**Model Name:** [Name of the AI model/system]  
**Version:** [e.g., v1.0, v2.1]  
**Date Created:** [YYYY-MM-DD]  
**Last Updated:** [YYYY-MM-DD]  
**Model Owner:** [Name and contact]  
**Data Owner:** [Name and contact]  
**Documentation Owner:** [Name and contact]  

---

## Executive Summary

[1-2 paragraph description of what the model does, its primary use case, and intended users]

**Example**: "The Staff Copilot is a generative AI assistant trained on publicly available documentation and organizational best practices. It helps employees draft communications, summarize documents, and answer policy questions. It is not trained on confidential customer or patient data."

---

## Model Details

### Architecture & Technical Approach
- **Model Type:** [e.g., Supervised Learning, Generative AI, Ensemble, etc.]
- **Algorithm/Architecture:** [e.g., Random Forest, Transformer, Logistic Regression]
- **Framework & Libraries:** [e.g., PyTorch, TensorFlow, scikit-learn]
- **Model Size:** [e.g., 175B parameters, 50MB file size]
- **Inference Latency:** [e.g., 200ms average]
- **Hardware Requirements:** [e.g., GPU/CPU, memory, storage]

### Training Approach
- **Training Data Source:** [Where training data came from]
- **Data Collection Period:** [Date range]
- **Training Dataset Size:** [e.g., 1M samples]
- **Data Filtering/Preprocessing:** [Any cleaning or filtering applied]
- **Feature Engineering:** [Key features used]
- **Hyperparameter Selection:** [Approach used - grid search, random search, etc.]
- **Training Environment:** [Infrastructure used]
- **Training Time:** [How long training took]

---

## Data

### Training Data Characteristics

**Dataset Overview:**
- **Total Samples:** [Number]
- **Features/Inputs:** [Number and types]
- **Labels/Outputs:** [Description]
- **Data Splits:** [e.g., 70% train, 15% validation, 15% test]
- **Class Balance:** [For classification: describe class distribution]
- **Missing Values:** [Percentage and handling method]

**Demographic Representation:**
- **Gender Representation:** [% breakdown if applicable]
- **Age Distribution:** [% breakdown if applicable]
- **Geographic Distribution:** [Coverage by region]
- **Socioeconomic Distribution:** [Income levels, etc. if applicable]
- **Underrepresented Groups:** [Known gaps in representation]

**Data Quality:**
- **Data Validation Rules:** [Quality checks applied]
- **Outlier Detection & Treatment:** [Approach used]
- **Temporal Coverage:** [Date range]
- **Data Lineage:** [Traceability documented]

### Known Data Limitations
- [List any known data quality issues, biases, or limitations]
- [Document time period bias if data is temporally specific]
- [Note any geographic limitations]
- [Document underrepresented populations]

---

## Performance

### Overall Performance

**Primary Metrics:**
| Metric | Value | Test Set | Notes |
|--------|-------|----------|-------|
| Accuracy | XX.X% | Held-out test set | [Any important notes] |
| Precision | XX.X% | Held-out test set | [For classification] |
| Recall | XX.X% | Held-out test set | [For classification] |
| F1-Score | XX.X% | Held-out test set | [Harmonic mean] |
| RMSE | X.XX | Held-out test set | [For regression] |
| AUC-ROC | X.XX | Held-out test set | [For ranking] |

**Secondary Metrics:**
| Metric | Value | Notes |
|--------|-------|-------|
| | | |

### Disaggregated Performance

**Performance by Demographic Group:**
| Group | Sample Size | Accuracy | Precision | Recall | F1-Score | Notes |
|-------|-------------|----------|-----------|--------|----------|-------|
| Overall | X,XXX | XX.X% | XX.X% | XX.X% | XX.X% | Baseline |
| [Group 1] | X,XXX | XX.X% | XX.X% | XX.X% | XX.X% | [Disparity noted?] |
| [Group 2] | X,XXX | XX.X% | XX.X% | XX.X% | XX.X% | [Disparity noted?] |
| [Group 3] | X,XXX | XX.X% | XX.X% | XX.X% | XX.X% | [Disparity noted?] |

**Performance by Input Subgroup:**
| Input Characteristic | Sample Size | Performance | Notes |
|---------------------|-------------|-------------|-------|
| [Low values] | X,XXX | XX.X% | Performance degradation? |
| [High values] | X,XXX | XX.X% | Performance degradation? |
| [Rare values] | X,XXX | XX.X% | Hard-to-predict cases? |

### Fairness Analysis

**Fairness Metrics:**
- **Disparate Impact Ratio:** [Ratio of favorable outcomes for protected vs. non-protected groups]
- **Equal Opportunity Difference:** [False Positive Rate difference across groups]
- **Demographic Parity:** [% difference in positive outcomes across groups]
- **Calibration:** [Does confidence score match actual accuracy across groups?]

**Fairness Assessment:**
- [ ] Model meets fairness thresholds
- [ ] Known fairness disparities identified: [List]
- [ ] Fairness mitigation strategies implemented: [List]
- [ ] Fairness trade-offs documented: [List]

### Error Analysis

**Common Error Patterns:**
- [Pattern 1]: Frequency X%, impact level [high/medium/low]
- [Pattern 2]: Frequency X%, impact level [high/medium/low]
- [Pattern 3]: Frequency X%, impact level [high/medium/low]

**Failure Cases:**
- [Edge case 1 and mitigation]
- [Edge case 2 and mitigation]
- [Minority population case and mitigation]

---

## Limitations & Known Issues

### Model Limitations
- [Limitation 1]
- [Limitation 2]
- [Limitation 3]

### Bias & Fairness Concerns
- [Known bias 1: description and impact]
- [Known bias 2: description and impact]
- [Mitigation strategies in place or planned]

### Adversarial Robustness
- **Adversarial Testing Conducted:** [ Yes / No ]
- **Known Vulnerabilities:** [List any known adversarial attacks that work]
- **Robustness Improvements:** [Planned or implemented]

### Out-of-Distribution Performance
- **Performance on distribution shift:** [How does model perform on data different from training?]
- **Known failure scenarios:** [Describe]

---

## Recommended Use & Constraints

### Intended Use Cases
- Primary use case: [Description]
- Secondary use cases: [If applicable]
- Intended users: [Who should use this model]
- Deployment context: [Where/how the model is deployed]

### Appropriate Use Constraints
- **Do use the model for:**
  - [ ] [Specific use case]
  - [ ] [Specific use case]
- **Don't use the model for:**
  - [ ] [High-stakes individual decisions without human review]
  - [ ] [Prediction on populations not represented in training data]
  - [ ] [Use case not tested]

### Special Monitoring Requirements
- [If used for Group A, monitor for ...]
- [If used for high-stakes decisions, ...]
- [Required human review thresholds: ...]

---

## Human Oversight

### Required Human Review
- **Threshold:** [When human review is mandatory]
- **Review SLA:** [Time to complete review]
- **Appeal Process:** [How can individuals appeal decisions?]
- **Decision Override Rate Target:** [Acceptable rate of model override]

### Human Reviewer Training
- **Training Content:** [What reviewers must know]
- **Training Frequency:** [Annual / biennial / etc.]
- **Competency Assessment:** [How reviewer competency is validated]

---

## Monitoring & Maintenance

### Monitoring Plan
- **Metrics Tracked:** [List KPIs]
- **Monitoring Frequency:** [Real-time / daily / weekly / monthly]
- **Performance SLA:** [Expected accuracy ±X%]
- **Fairness SLA:** [Acceptable disparity threshold]
- **Drift Detection:** [How model drift is detected]

### Retraining Triggers
- [ ] Performance drops below X%
- [ ] Fairness metric breaches threshold
- [ ] Data distribution shift detected (KL divergence > X)
- [ ] Scheduled quarterly retraining
- [ ] New data volume exceeds X samples
- [ ] [Other trigger]: [Description]

### Retraining Process
- **Retraining Frequency:** [When model is retrained]
- **Retraining Data:** [How new training data is selected]
- **Validation Steps:** [Testing required before deployment]
- **Rollback Plan:** [How to revert to previous version if needed]

---

## Compliance & Governance

### Regulatory Classification
- **NIST AI RMF Risk Category:** [Impact / Performance / Security / Fairness risk levels]
- **EU AI Act Risk Tier:** [Prohibited / High-Risk / Limited Risk / Minimal Risk]
- **Applicable Regulations:** [GDPR / HIPAA / Fair Lending Laws / etc.]

### Governance
- **AI Governance Status:** [Approved / Under Review / Requires Improvement]
- **Last Governance Review:** [Date]
- **Next Governance Review:** [Date]
- **Outstanding Issues:** [Any governance gaps]

### Documentation
- **Risk Assessment:** [Completed / Location]
- **Impact Assessment:** [DPIA / Location]
- **Fairness Audit:** [Completed / Location]
- **Conformity Assessment:** [Completed / Location]
- **Third-Party Review:** [Completed / Date / Assessor]

---

## Contact & Support

**For Questions About This Model:**
- Technical Questions: [Name, email]
- Governance/Compliance: [Name, email]
- Monitoring/Operational Issues: [Name, email]

**Model Repository Location:** [GitHub URL or internal location]  
**Documentation Location:** [Wiki or doc repository URL]  
**Issue Tracking:** [Jira / GitHub Issues / etc.]

---

## Version History

| Version | Date | Changes | Owner |
|---------|------|---------|-------|
| v1.0 | YYYY-MM-DD | Initial release | [Name] |
| v2.0 | YYYY-MM-DD | Fairness improvements, retraining | [Name] |
| [Current] | YYYY-MM-DD | [Brief description] | [Name] |

---

**Template Version**: 1.0  
**Last Updated**: September 2026  
**Compatible With**: NIST AI RMF 1.0 | ISO/IEC 42001:2023 | EU AI Act (2024/1689)

---

## Additional Notes

[Any other important information not covered above]

---

**Approval Sign-off**

- [ ] Model Owner Approved: _________________ Date: _______
- [ ] Data Owner Approved: _________________ Date: _______
- [ ] AI Governance Approved: _________________ Date: _______
- [ ] Compliance/Legal Review (if required): _________________ Date: _______
