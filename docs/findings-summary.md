# Cyber Risk Findings Summary

## Overview

The assessment identified three cybersecurity risk scenarios within the defined Check Point R82 laboratory scope.

| Risk ID | Risk Scenario | Current Score | Current Level | Target Score | Target Level | Treatment |
|---|---|---:|---|---:|---|---|
| RISK-001 | IPS protection currency limitation | 12 | High | 8 | Medium | Mitigate |
| RISK-002 | SQL Injection protection effectiveness not conclusively validated | 12 | High | 8 | Medium | Mitigate |
| RISK-003 | Broad network access within the laboratory environment | 6 | Medium | 3 | Low | Mitigate |

No Critical risks were identified.

---

## RISK-001 — IPS Protection Currency Limitation

### Risk Scenario

The IPS protection database could not be updated under the observed Security Gateway connectivity condition.

Although IPS was enabled and the relevant protection profile was active, inability to maintain protection currency may reduce coverage against newer threats.

### Current Risk

- **Likelihood:** 3 — Possible
- **Impact:** 4 — Major
- **Risk Score:** 12
- **Risk Level:** High

### Existing Controls

- IPS enabled
- LAB-IPS-Detect profile active
- Threat Prevention enabled
- Security policy deployed

### Treatment

Restore controlled Internet connectivity required for IPS updates, update the IPS protection database, and establish periodic verification of protection currency.

### Target Risk

- **Target Likelihood:** 2 — Unlikely
- **Target Impact:** 4 — Major
- **Target Risk Score:** 8
- **Target Risk Level:** Medium

The target rating assumes successful remediation and validation. It does not represent confirmed residual risk.

---

## RISK-002 — SQL Injection Protection Effectiveness

### Risk Scenario

SQL Injection protection was configured as **Drop + Log**, but effective blocking could not be conclusively demonstrated during controlled testing.

The control therefore existed and was configured, but its operating effectiveness required additional validation.

### Current Risk

- **Likelihood:** 3 — Possible
- **Impact:** 4 — Major
- **Risk Score:** 12
- **Risk Level:** High

### Existing Controls

- IPS enabled
- SQL Injection protection configured
- Drop + Log action configured
- Threat Prevention policy deployed
- Security logging enabled

### Treatment

Perform controlled SQL Injection testing, verify blocking and logging behavior, validate security logs, and document evidence demonstrating operating effectiveness.

### Target Risk

- **Target Likelihood:** 2 — Unlikely
- **Target Impact:** 4 — Major
- **Target Risk Score:** 8
- **Target Risk Level:** Medium

The target rating is conditional upon successful control validation.

---

## RISK-003 — Broad Network Access

### Risk Scenario

Broad network access was intentionally permitted within the laboratory environment to support security testing.

While this was acceptable for the defined lab scenario, equivalent access in a production environment could increase exposure to unauthorized network communication.

### Current Risk

- **Likelihood:** 2 — Unlikely
- **Impact:** 3 — Moderate
- **Risk Score:** 6
- **Risk Level:** Medium

### Existing Controls

- Check Point Access Control policy
- Security logging
- IPS
- Threat Prevention
- Network segmentation within the laboratory

### Treatment

Review firewall rules according to least-privilege principles, restrict unnecessary destinations and services, document business justification for broad access, and perform periodic firewall rule reviews.

### Target Risk

- **Target Likelihood:** 1 — Rare
- **Target Impact:** 3 — Moderate
- **Target Risk Score:** 3
- **Target Risk Level:** Low

The target rating assumes that access restrictions have been implemented and validated.

---

## Risk Reduction Overview

Following successful implementation and validation of the recommended treatments, the modeled risk profile changes from:

- **2 High**
- **1 Medium**
- **0 Critical**

to:

- **0 High**
- **2 Medium**
- **1 Low**
- **0 Critical**

This represents the expected target state rather than confirmed post-remediation residual risk.

## Assessment Perspective

The assessment demonstrates that the existence of a security control does not, by itself, establish control effectiveness.

Technical configuration, operating behavior, supporting evidence, and identified limitations were considered when translating security observations into risk-management decisions.
