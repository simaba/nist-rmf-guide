# EU AI Act ↔ NIST AI RMF Cross-Reference

This document maps requirements from the EU AI Act (Regulation 2024/1689)
to the corresponding NIST AI RMF functions and subcategories.

> **Purpose:** Organizations subject to the EU AI Act can use this mapping to
> understand which NIST AI RMF practices also satisfy EU AI Act obligations.
> Organizations implementing NIST AI RMF can assess their EU AI Act readiness.

---

## Risk Classification Alignment

| EU AI Act Risk Tier | NIST AI RMF Equivalent | Treatment |
|---|---|---|
| Unacceptable Risk (Art. 5) | Prohibited use cases | Governance policy must explicitly prohibit |
| High Risk (Annex III) | High-risk AI systems | Full GOVERN + MAP + MEASURE + MANAGE cycle |
| Limited Risk (Art. 50) | Medium-risk AI systems | Transparency obligations; streamlined governance |
| Minimal Risk | Low-risk AI systems | Voluntary best practices only |

---

## High-Risk AI System Requirements (Annex III)

High-risk AI system categories under EU AI Act Annex III include:
- Biometric identification and categorization
- Critical infrastructure management
- Education and vocational training
- Employment and worker management
- Access to essential services (credit, insurance, social benefits)
- Law enforcement
- Migration, asylum, and border control
- Administration of justice

### Article 9 — Risk Management System

| EU AI Act Requirement | NIST AI RMF Mapping | Implementation |
|---|---|---|
| Continuous risk management process | GV.1, GV.6, MP.4, MS.2 | Ongoing governance committee reviews |
| Identification and analysis of known risks | MP.3, MP.4 | Risk register maintenance |
| Risk evaluation post-deployment | MS.2, MG.3 | Production monitoring and alerting |
| Risk mitigation measures | MG.2, MG.4 | Risk treatment documentation |

### Article 10 — Data and Data Governance

| EU AI Act Requirement | NIST AI RMF Mapping | Implementation |
|---|---|---|
| Training data practices documented | MP.2, MS.1 | Dataset documentation / datasheets |
| Relevance and representativeness assessed | MS.1, MS.5 | Bias evaluation reports |
| Known biases identified and addressed | MS.5, MG.2 | Fairness testing, subgroup analysis |
| Data governance practices in place | GV.1, GV.3 | Data governance policy |

### Article 11 — Technical Documentation

| EU AI Act Requirement | NIST AI RMF Mapping | Implementation |
|---|---|---|
| System description and intended purpose | MP.1, MP.2 | Model card — system description section |
| Design specifications | MP.3 | Architecture documentation |
| Training methodology and datasets | MP.2, MS.1 | Model card — training section |
| Performance metrics and testing results | MS.3, MS.4 | Evaluation reports |
| Risk management documentation | MG.1, MG.2 | Risk register and treatment plans |

### Article 13 — Transparency and Provision of Information

| EU AI Act Requirement | NIST AI RMF Mapping | Implementation |
|---|---|---|
| Instructions for use (operators) | GV.5, MP.5 | Operational documentation |
| Limitations and known risks disclosed | MP.4, MS.5 | Model card — limitations section |
| Human oversight requirements | GV.4, MG.4 | Human-in-the-loop documentation |
| Performance in specific groups | MS.5 | Subgroup performance analysis |

### Article 14 — Human Oversight

| EU AI Act Requirement | NIST AI RMF Mapping | Implementation |
|---|---|---|
| Human oversight measures designed in | GV.4, MG.4 | Human oversight protocols |
| Operators can understand system behavior | GV.5, MS.1 | Explainability documentation |
| Override / suspend capability | MG.4 | Kill switch / override procedures |
| Automated alert for anomalies | MS.2, MG.3 | Monitoring and alerting setup |

---

## Prohibited AI Practices (Article 5) — GOVERN Alignment

The following uses are prohibited under EU AI Act Article 5.
Your GOVERN function policies must explicitly prohibit these:

- Subliminal manipulation techniques
- Exploitation of vulnerabilities of specific groups
- Social scoring by public authorities
- Real-time remote biometric identification in public spaces (with limited exceptions)
- Emotion recognition in workplace or educational settings
- AI-generated or manipulated content without transparency (deepfakes)

**Implementation:** Add a "Prohibited AI Uses" section to your AI governance policy
(see [templates/ai-governance-policy.md](../templates/ai-governance-policy.md)).

---

## Conformity Assessment

For high-risk AI systems (Annex III), EU AI Act requires conformity assessment before deployment:

| AI System Type | Assessment Method |
|---|---|
| Biometric identification | Third-party conformity assessment (notified body) |
| Most other Annex III systems | Self-assessment with technical documentation |

**NIST AI RMF alignment:** The full MAP → MEASURE → MANAGE cycle, documented with
the templates in this repository, constitutes strong evidence for self-assessment conformity.

---

## Timeline

| Date | EU AI Act Milestone |
|---|---|
| August 2024 | Regulation entered into force |
| February 2025 | Prohibited practices apply |
| August 2025 | GPAI model provisions apply |
| August 2026 | High-risk system obligations apply (most Annex III) |
| August 2027 | High-risk systems (Annex I) obligations apply |

---

*This mapping is provided for informational purposes and does not constitute legal advice.
Consult qualified EU AI Act legal counsel for compliance decisions.*
