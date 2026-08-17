# Cyber Risk Assessment Methodology

## 1. Purpose

This assessment translates technical security observations from a controlled Check Point R82 cybersecurity laboratory into structured cyber risk scenarios, control assessments, remediation actions, and management-level risk reporting.

The objective is to demonstrate an evidence-based approach in which technical findings are connected to assets, security controls, business/security impact, risk treatment, and target residual risk.

## 2. Assessment Approach

The assessment followed the sequence:

Technical Observation → Asset → Control → Evidence → Risk Scenario → Risk Rating → Treatment → Target Risk

Each risk scenario was evaluated using documented technical evidence and the security controls observed within the laboratory environment.

## 3. Risk Assessment Model

Risk was evaluated using a 5×5 likelihood-impact matrix.

### Likelihood

| Score | Rating |
|---|---|
| 1 | Rare |
| 2 | Unlikely |
| 3 | Possible |
| 4 | Likely |
| 5 | Almost Certain |

### Impact

| Score | Rating |
|---|---|
| 1 | Insignificant |
| 2 | Minor |
| 3 | Moderate |
| 4 | Major |
| 5 | Severe |

Risk score was calculated as:

**Risk Score = Likelihood × Impact**

### Risk Rating

| Score | Risk Level |
|---|---|
| 1–4 | Low |
| 5–9 | Medium |
| 10–16 | High |
| 17–25 | Critical |

## 4. Control Assessment

Security controls were evaluated using configuration evidence, technical observations, command-line output, controlled testing, and security policy review.

Control implementation and control effectiveness were considered separately. A control being configured or enabled was not automatically considered evidence that its operating effectiveness had been conclusively demonstrated.

## 5. Evidence-Based Assessment

Evidence was mapped to relevant assets, controls, findings, and risk scenarios to provide traceability across the assessment.

Evidence limitations were documented where technical validation could not conclusively demonstrate control effectiveness.

## 6. Risk Treatment

Identified risks were assigned treatment actions based on the observed control limitations and assessed exposure.

Recommended remediation activities were designed to reduce either the likelihood or impact of the associated risk scenario.

## 7. Target Residual Risk

Target residual risk represents the expected risk level following successful implementation and validation of the recommended remediation actions.

Target residual risk should not be interpreted as confirmed residual risk until remediation has been completed and supporting evidence has been reviewed.

## 8. Assessment Limitations

This project was conducted in a controlled cybersecurity laboratory environment and does not represent a production infrastructure assessment.

The results demonstrate the assessment methodology and technical-to-risk traceability within the defined laboratory scope.
