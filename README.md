# NIST AI RMF Implementation Guide

[![NIST AI RMF 1.0](https://img.shields.io/badge/NIST%20AI%20RMF-1.0-0055A4?style=for-the-badge)](https://airc.nist.gov/home)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)
[![Maintained](https://img.shields.io/badge/Maintained-yes-green.svg?style=flat-square)](https://github.com/simaba/nist-rmf-guide)
[![Discussions](https://img.shields.io/badge/GitHub-Discussions-7289da?style=flat-square&logo=github)](https://github.com/simaba/nist-rmf-guide/discussions)

A practitioner's implementation guide for the NIST AI Risk Management Framework (AI RMF 1.0).

## Choose this repo when

Use this repository when you need help translating the **NIST AI RMF itself** into practical actions, templates, and implementation sequences.

Use a different repo when you need:

- the broader AI operating model: [`governance-playbook`](https://github.com/simaba/governance-playbook)
- release-stage lifecycle governance: [`release-governance`](https://github.com/simaba/release-governance)
- a working release-readiness validator: [`release-checklist`](https://github.com/simaba/release-checklist)
- a starter template repo: [`regulated-ai`](https://github.com/simaba/regulated-ai)

> This guide is maintained by a practitioner, not NIST. Always refer to the official NIST documentation for authoritative language.

## Maturity

This is a **practitioner implementation guide**. It is designed to help teams structure gap assessments, templates, implementation sequences, and internal discussions. It is not an official NIST document, audit result, compliance certification, or regulatory determination.

## Practical start point

If you already have AI systems and want to identify gaps, start here:

| Artifact | Use for |
|---|---|
| [`templates/nist-rmf-gap-assessment.md`](templates/nist-rmf-gap-assessment.md) | Assessing current maturity across Govern, Map, Measure, and Manage |
| [`examples/sample-nist-rmf-gap-assessment.md`](examples/sample-nist-rmf-gap-assessment.md) | Seeing a filled generic example of an RMF-style gap assessment |

## Guide structure

| Section | What you will find |
|---|---|
| [01 - Govern](docs/01-govern.md) | Policies, roles, accountability structures |
| [02 - Map](docs/02-map.md) | Risk categorization, context setting, stakeholder identification |
| [03 - Measure](docs/03-measure.md) | Risk analysis methods, evaluation metrics, testing approaches |
| [04 - Manage](docs/04-manage.md) | Risk response, prioritization, residual risk acceptance |
| [Templates](templates/) | Ready-to-use document templates |
| [Examples](examples/) | Industry-specific implementation examples |
| [Tools](tools/) | Scripts and utilities for automated governance checks |
| [EU AI Act Mapping](docs/eu-ai-act-mapping.md) | Practitioner cross-reference between NIST AI RMF and EU AI Act concepts |
| [ISO 42001 Mapping](docs/iso-42001-mapping.md) | Practitioner cross-reference with ISO/IEC 42001 |

## Quick start

### If you are starting from scratch

1. Read [01 - Govern](docs/01-govern.md)
2. Complete the [Model Inventory Template](templates/model-inventory.md)
3. Run through [02 - Map](docs/02-map.md) for your highest-risk AI system
4. Use the [Risk Assessment Template](templates/risk-assessment.md)

### If you have existing AI systems

1. Start with the [NIST AI RMF Gap Assessment Template](templates/nist-rmf-gap-assessment.md)
2. Compare against the [sample gap assessment](examples/sample-nist-rmf-gap-assessment.md)
3. Use [03 - Measure](docs/03-measure.md) to evaluate current controls
4. Prioritize gaps using the [Risk Register Template](templates/risk-register.md)

### If you are preparing for compliance

1. Review the [EU AI Act Mapping](docs/eu-ai-act-mapping.md)
2. Check the [ISO 42001 Mapping](docs/iso-42001-mapping.md)
3. Use the [Governance Checklist](templates/governance-checklist.md)
4. Verify all interpretations against official sources and qualified internal reviewers before using them for compliance decisions

## Scope and disclaimer

This repository is shared in a personal capacity. It is not legal advice, compliance certification, regulatory approval, safety certification, audit evidence, or official guidance from NIST, the EU, ISO, or any employer.

References to NIST AI RMF, EU AI Act, ISO/IEC 42001, governance controls, or regulated-industry obligations are practitioner mappings and examples. Always verify against official sources and internal requirements before using this guide for compliance, safety, or release decisions.

## Related repositories

| Repository | What it adds |
|---|---|
| [governance-playbook](https://github.com/simaba/governance-playbook) | Broader operating model |
| [release-governance](https://github.com/simaba/release-governance) | Release lifecycle governance |
| [release-checklist](https://github.com/simaba/release-checklist) | Working release-readiness validator |
| [regulated-ai](https://github.com/simaba/regulated-ai) | Starter template repo |
| [ai-prism](https://github.com/simaba/ai-prism) | Curated standards, tools, and papers |

## License

MIT License. This guide is not affiliated with or endorsed by NIST.
