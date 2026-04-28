# NIST AI RMF Gap Assessment

This example is generic and illustrative. It is not an official NIST artifact and does not describe a real organization.

## 1. Assessment Metadata

| Field | Value |
|---|---|
| Organization / team | Example AI Product Team |
| AI system or portfolio | Document Triage Assistant |
| Assessment date | 2026-04-26 |
| Assessor | Example AI Governance Lead |
| Scope | Single system |
| Risk tier | Medium |
| Review cadence | Quarterly |

## 2. Summary Rating

| RMF Function | Current maturity | Target maturity | Gap severity | Priority |
|---|---:|---:|---|---|
| Govern | 2 | 4 | Medium | High |
| Map | 3 | 4 | Medium | Medium |
| Measure | 2 | 4 | High | High |
| Manage | 2 | 4 | High | High |

## 3. Govern

| Control area | Current state | Evidence | Gap | Action owner | Due date |
|---|---|---|---|---|---|
| AI policy and principles | documented at team level | draft AI policy | not yet approved enterprise-wide | Governance Lead | 2026-05-30 |
| Roles and accountability | business and technical owners assigned | model inventory draft | backup owners missing | Product Owner | 2026-05-10 |
| System inventory | one system listed | model inventory | dependency details incomplete | Technical Owner | 2026-05-17 |
| Risk-tiering process | medium risk assigned | risk assessment draft | tiering criteria not standardized | Risk Owner | 2026-05-24 |
| Governance review cadence | quarterly proposed | meeting plan | not yet operating | Governance Lead | 2026-06-01 |

## 4. Map

| Control area | Current state | Evidence | Gap | Action owner | Due date |
|---|---|---|---|---|---|
| Use-case context | documented for staging release | use-case summary | production scope not finalized | Product Owner | 2026-05-10 |
| Stakeholder and impact mapping | main user groups identified | stakeholder map | affected downstream teams not fully reviewed | Product Owner | 2026-05-17 |
| Data and dependency mapping | primary input sources listed | architecture note | vendor and logging dependencies need detail | Technical Owner | 2026-05-24 |
| Harm and failure-mode identification | initial failure modes captured | risk register | sensitive-case escalation scenarios incomplete | Risk Owner | 2026-05-10 |
| Regulatory or policy context | preliminary review done | privacy checklist | legal review still pending | Legal Reviewer | 2026-05-30 |

## 5. Measure

| Control area | Current state | Evidence | Gap | Action owner | Due date |
|---|---|---|---|---|---|
| Performance evaluation | benchmark run completed | evaluation report | limited sample size | ML Owner | 2026-05-17 |
| Fairness and subgroup testing | not yet complete | none | subgroup performance not measured | ML Owner | 2026-05-24 |
| Robustness and red-team testing | partial prompt-injection tests | test log | no sensitive-case regression pack | Risk Owner | 2026-05-17 |
| Monitoring and drift metrics | proposed metrics listed | monitoring draft | thresholds not approved | Operations Owner | 2026-05-20 |
| Traceability and auditability | trace IDs planned | logging design | retention and masking policy incomplete | Data Owner | 2026-05-30 |

## 6. Manage

| Control area | Current state | Evidence | Gap | Action owner | Due date |
|---|---|---|---|---|---|
| Risk treatment plan | high-priority risks listed | risk register | action owners not confirmed for all items | Risk Owner | 2026-05-10 |
| Release gate decision process | staging gate planned | release-gate agenda | production gate criteria unclear | Release Owner | 2026-05-17 |
| Incident response and escalation | draft runbook exists | incident playbook draft | tabletop exercise not run | Operations Owner | 2026-05-24 |
| Post-release review | quarterly review proposed | governance calendar | metrics not yet tied to review decisions | Governance Lead | 2026-06-01 |
| Retirement or rollback criteria | rollback owner named | release checklist | rollback trigger not tested | Platform Owner | 2026-05-24 |

## 7. Top Gaps

| Gap | RMF function | Severity | Recommended action | Owner | Due date |
|---|---|---|---|---|---|
| subgroup performance not measured | Measure | High | add subgroup test set and report results | ML Owner | 2026-05-24 |
| sensitive-case escalation scenarios incomplete | Map / Measure | High | create regression pack for sensitive cases | Risk Owner | 2026-05-17 |
| incident response not tested | Manage | High | run tabletop exercise before production gate | Operations Owner | 2026-05-24 |
| retention and masking policy incomplete | Measure / Govern | Medium | approve logging and retention policy | Data Owner | 2026-05-30 |

## 8. Improvement Roadmap

### Next 30 days

- finalize owner and backup-owner assignments
- complete sensitive-case regression scenarios
- run subgroup performance evaluation
- confirm rollback trigger and incident escalation path

### Next 90 days

- standardize risk-tiering criteria
- run a tabletop incident exercise
- connect monitoring metrics to governance review decisions
- complete legal and privacy review

### Next 180 days

- move from team-level controls to standardized portfolio controls
- create reusable evidence package for repeated release gates
- review whether the system should remain medium risk or be re-tiered

## 9. Review Decision

- [ ] Current controls acceptable for scope
- [x] Acceptable with remediation plan
- [ ] Not acceptable until high-severity gaps are closed

Decision rationale:

The system can proceed with controlled staging use, but production release should remain conditional until high-severity Measure and Manage gaps are closed.
