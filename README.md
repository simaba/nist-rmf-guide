# NIST AI RMF Implementation Guide

[![NIST AI RMF 1.0](https://img.shields.io/badge/NIST%20AI%20RMF-1.0-0055A4?style=for-the-badge)](https://airc.nist.gov/home)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)
[![Maintained](https://img.shields.io/badge/Maintained-yes-green.svg?style=flat-square)](https://github.com/simaba/nist-rmf-guide)
[![Discussions](https://img.shields.io/badge/GitHub-Discussions-7289da?style=flat-square&logo=github)](https://github.com/simaba/nist-rmf-guide/discussions)

**A practitioner's implementation guide for the NIST AI Risk Management Framework (AI RMF 1.0).**

The official NIST AI RMF documentation is comprehensive but abstract. This guide translates the framework into **concrete actions, checklists, code examples, and templates** that engineering and governance teams can use directly.

> This guide is maintained by an AI governance practitioner, not NIST. It reflects a practitioner's interpretation of the framework. Always refer to the [official NIST AI RMF documentation](https://www.nist.gov/artificial-intelligence/ai-risk-management-framework) for authoritative guidance.

---

## What Is the NIST AI RMF?

The NIST AI Risk Management Framework (AI RMF 1.0, January 2023) is a voluntary framework for managing risks across the AI system lifecycle. It is organized around four core functions:

```text
┌─────────────┐     ┌─────────────┐     ┌─────────────┐     ┌─────────────┐
│   GOVERN    │ ──► │     MAP     │ ──► │   MEASURE   │ ──► │   MANAGE    │
│             │     │             │     │             │     │             │
│ Policies,   │     │ Categorize  │     │ Evaluate &  │     │ Prioritize  │
│ culture,    │     │ & contextu- │     │ analyze     │     │ & respond   │
│ roles       │     │ alize risks │     │ risks       │     │ to risks    │
└─────────────┘     └─────────────┘     └─────────────┘     └─────────────┘
```

---

## Guide Structure

| Section | What You Will Find |
|---|---|
| [01 - Govern](docs/01-govern.md) | Policies, organizational culture, roles, accountability structures |
| [02 - Map](docs/02-map.md) | Risk categorization, context setting, stakeholder identification |
| [03 - Measure](docs/03-measure.md) | Risk analysis methods, evaluation metrics, testing approaches |
| [04 - Manage](docs/04-manage.md) | Risk response, prioritization, residual risk acceptance |
| [Templates](templates/) | Ready-to-use document templates for each function |
| [Examples](examples/) | Industry-specific implementation examples (healthcare, finance, insurance) |
| [Tools](tools/) | Scripts and utilities for automated governance checks |
| [EU AI Act Mapping](docs/eu-ai-act-mapping.md) | Cross-reference between NIST AI RMF and EU AI Act requirements |
| [ISO 42001 Mapping](docs/iso-42001-mapping.md) | Cross-reference with ISO/IEC 42001 AI management system standard |

---

## Quick Start: Where to Begin

### If you are starting from scratch:
1. Read [01 - Govern](docs/01-govern.md) to establish who owns AI governance.
2. Complete the [Model Inventory Template](templates/model-inventory.md).
3. Run through [02 - Map](docs/02-map.md) for your highest-risk AI system.
4. Use the [Risk Assessment Template](templates/risk-assessment.md).

### If you have existing AI systems:
1. Start with [02 - Map](docs/02-map.md) to categorize your current systems.
2. Use the [Risk Assessment Template](templates/risk-assessment.md) to identify governance gaps.
3. Use [03 - Measure](docs/03-measure.md) to evaluate your current controls.
4. Prioritize gaps using the [Risk Register Template](templates/risk-register.md).

### If you are preparing for compliance:
1. Review the [EU AI Act Mapping](docs/eu-ai-act-mapping.md) if EU-facing.
2. Check the [ISO 42001 Mapping](docs/iso-42001-mapping.md) for certification readiness.
3. Use the [Governance Checklist](templates/governance-checklist.md) for a gap assessment.

---

## The Seven Characteristics of Trustworthy AI

The NIST AI RMF is built around seven characteristics that trustworthy AI systems should exhibit. This guide provides practical implementation guidance for each:

| Characteristic | Description | Key Practices |
|---|---|---|
| **Accountable** | Clear responsibility for AI system outcomes | Roles & responsibilities, audit trails, model inventory |
| **Explainable** | AI decisions can be understood and communicated | Explainability reports, model cards, documentation |
| **Interpretable** | Meaning of outputs can be understood | Feature importance, decision logs, SHAP/LIME integration |
| **Privacy-Enhanced** | Privacy risks are managed and minimized | Data minimization, PII handling, consent management |
| **Reliable** | Consistent performance within expected conditions | Performance monitoring, regression testing, drift detection |
| **Safe** | Does not cause undue harm to people or systems | Red teaming, adversarial testing, failure mode analysis |
| **Secure & Resilient** | Resistant to attacks and recovers from failures | Security scanning, penetration testing, incident response |
| **Fair** | Equitable outcomes across affected populations | Bias evaluation, disparate impact analysis, subgroup testing |

---

## GOVERN Function — Getting Started

The GOVERN function establishes the organizational context for AI risk management. Key implementation steps:

1. **Assign AI governance ownership** — designate an AI governance lead or committee
2. **Document AI use policies** — what AI is allowed and not allowed at your organization
3. **Create a model inventory** — maintain a current list of all AI systems in operation
4. **Establish risk tolerance** — define acceptable risk levels for different AI use cases
5. **Implement training** — ensure all AI practitioners understand governance requirements

See [docs/01-govern.md](docs/01-govern.md) for full implementation guidance.

---

## Ecosystem

This guide is part of a broader AI governance framework:

| Repository | Purpose |
|---|---|
| [governance-playbook](https://github.com/simaba/governance-playbook) | End-to-end governance playbook |
| [release-checklist](https://github.com/simaba/release-checklist) | Release gate framework |
| [release-governance](https://github.com/simaba/release-governance) | Release lifecycle governance |
| [regulated-ai](https://github.com/simaba/regulated-ai) | Starter repository for regulated AI teams |
| [ai-prism](https://github.com/simaba/ai-prism) | Curated resource list |

---

## Contributing

This guide improves through practitioner feedback. If you have implemented NIST AI RMF and have insights to share, see [CONTRIBUTING.md](CONTRIBUTING.md).

Especially valuable:
- Industry-specific implementation examples
- Corrections to interpretations
- Additional tool integrations
- Case studies (anonymized)

---

## License

MIT License — use and adapt freely with attribution.

*This guide is not affiliated with or endorsed by NIST.*
