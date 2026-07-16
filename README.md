# NIST AI RMF Practitioner Guide

[![NIST AI RMF 1.0](https://img.shields.io/badge/NIST%20AI%20RMF-1.0-0055A4?style=flat-square)](https://airc.nist.gov/home)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)

A practitioner guide for navigating the NIST AI Risk Management Framework and turning selected official references into scoped internal questions, evidence needs, decisions, and improvement work.

This repository is not an official NIST implementation guide. Completing its templates does not establish AI RMF implementation, maturity, compliance, or control effectiveness.

## Start from the official source

Use the official NIST AI RMF and related NIST resources as the authoritative material. For each internal review:

1. identify the function, category, and subcategory relevant to the system and decision;
2. preserve the official reference and version;
3. translate it into a proposition the organization can assess;
4. define the system scope, population, evidence, owner, and decision consequence;
5. record uncertainty, gaps, and not-applicable rationale;
6. revisit the conclusion when the system, context, or source changes.

A generic checklist cannot determine applicability for every organization or use case.

## Practical start point

| Artifact | Use it for |
|---|---|
| [`templates/nist-rmf-gap-assessment.md`](templates/nist-rmf-gap-assessment.md) | evidence-based review across selected Govern, Map, Measure, and Manage references |
| [`examples/sample-nist-rmf-gap-assessment.md`](examples/sample-nist-rmf-gap-assessment.md) | fictional worked example to adapt critically |
| [`docs/01-govern.md`](docs/01-govern.md) | organizational decision rights, accountability, policy, and risk-management context |
| [`docs/02-map.md`](docs/02-map.md) | purpose, context, affected people, dependencies, benefits, and harms |
| [`docs/03-measure.md`](docs/03-measure.md) | measurement, evaluation, control evidence, and uncertainty |
| [`docs/04-manage.md`](docs/04-manage.md) | prioritization, treatment, decisions, monitoring, and response |
| [`docs/eu-ai-act-mapping.md`](docs/eu-ai-act-mapping.md) | practitioner cross-reference requiring verification against official legal sources |
| [`docs/iso-42001-mapping.md`](docs/iso-42001-mapping.md) | practitioner cross-reference requiring verification against official ISO material |

## Evidence, not function-level maturity scores

The revised assessment template does not assign one 0–5 maturity number to Govern, Map, Measure, or Manage.

A function-level score can hide important differences:

- policy exists but does not operate;
- one high-impact system has strong evidence while the rest of the portfolio is unknown;
- controls run but their outcomes are not measured;
- an artifact is complete but stale;
- a practice is partially demonstrated for one population and absent for another;
- a not-applicable judgment has no rationale.

Use evidence states instead:

| Status | Meaning |
|---|---|
| Demonstrated | current evidence shows operation for the reviewed scope |
| Partially demonstrated | evidence exists but material scope or limitations remain |
| Documented, not demonstrated | design or policy exists without sufficient operating evidence |
| Not demonstrated | required evidence or practice is absent |
| Not applicable | reviewed rationale supports exclusion for the scoped decision |
| Unknown | available evidence is insufficient to determine status |

Record whether evidence supports design, operation, or outcome. Those are different claims.

## Govern

Use Govern-related material to examine:

- decision, control, incident, exception, and residual-risk authority;
- policy scope and change management;
- roles, competence, and resources;
- system and dependency inventory;
- affected-party participation and accountability;
- supplier and third-party governance;
- documentation, communication, and review;
- organizational incentives and risk culture.

A named owner without authority or resources is not demonstrated accountability.

## Map

Use Map-related material to understand:

- intended use, prohibited use, users, and affected populations;
- operating environment and lifecycle stage;
- data, model, tool, supplier, and infrastructure dependencies;
- benefits and distribution of value;
- foreseeable misuse, failures, and harms;
- reversibility and remediation;
- legal, policy, sector, and organizational context;
- assumptions and evidence gaps.

Context should be revisited when authority, users, data, geography, or deployment changes.

## Measure

Use Measure-related material to examine:

- what property is being measured and for which decision;
- scenario and population coverage;
- evaluator validity;
- statistical and non-statistical uncertainty;
- disaggregated and affected-group outcomes;
- security, privacy, safety, reliability, and operational evidence;
- monitoring, incident, and control effectiveness;
- evidence provenance, freshness, and reproducibility.

A metric name such as accuracy, fairness, safety, or robustness is not an operational definition.

Companion repository: [`agent-eval`](https://github.com/simaba/agent-eval).

## Manage

Use Manage-related material to examine:

- risk prioritization and treatment;
- hard gates and decision outcomes;
- conditions, exceptions, and residual-risk acceptance;
- staged exposure and stop triggers;
- incident, containment, rollback, and remediation;
- monitoring and treatment effectiveness;
- renewal, change, and retirement;
- communication and redress.

A planned mitigation is not evidence that risk has been reduced.

Companion repository: [`release-governance`](https://github.com/simaba/release-governance).

## Gap assessment workflow

1. Define the lifecycle decision and exact system scope.
2. Select and record the relevant official references.
3. State the proposition each reference creates for the reviewed context.
4. Collect current evidence and provenance.
5. classify evidence state and limitations.
6. tie material gaps to a decision consequence.
7. distinguish blocker, required action, condition, exception, residual risk, and operating-model improvement.
8. record owner, due date or trigger, verification, and expiry.
9. state assessment limitations and unrepresented affected groups.

The output should explain what can and cannot be concluded—not produce an impressive-looking maturity number.

## Cross-framework mappings

The EU AI Act and ISO/IEC 42001 documents in this repository are practitioner navigation aids. They should not be used as substitute legal or standards text, and they do not establish equivalence between frameworks.

When using a mapping:

- verify the official source and current version;
- preserve differences in scope, legal effect, terminology, and evidence expectations;
- record where no direct correspondence exists;
- obtain qualified review for consequential interpretations;
- do not mark a requirement satisfied because a concept appears in another framework.

## Maturity and scope

This is a practitioner guide with templates and cross-references. It can support internal learning, scoped gap reviews, evidence planning, and operating-model discussions. It is not an audit, certification, compliance determination, legal opinion, safety case, or official NIST guidance.

## Related repositories

| Repository | Distinct role |
|---|---|
| [`governance-playbook`](https://github.com/simaba/governance-playbook) | enterprise decision and evidence operating model |
| [`release-governance`](https://github.com/simaba/release-governance) | release-stage evidence and decisions |
| [`release-checklist`](https://github.com/simaba/release-checklist) | executable release configuration validation |
| [`regulated-ai`](https://github.com/simaba/regulated-ai) | starter repository and templates |
| [`ai-prism`](https://github.com/simaba/ai-prism) | curated public resource hub |

---

*Practitioner guide maintained by [Sima Bagheri](https://github.com/simaba). Not affiliated with or endorsed by NIST.*
