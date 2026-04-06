# 01 — GOVERN Function

The GOVERN function establishes the organizational foundation for AI risk management.
It creates the policies, culture, and accountability structures that enable the other
three functions (Map, Measure, Manage) to operate effectively.

> **NIST AI RMF Definition:** Policies, processes, procedures, and practices across
> the organization related to the mapping, measuring, and managing of AI risks are in
> place, transparent, and implemented effectively.

---

## Key Categories

### GV.1 — Organizational Policies and Processes

**What NIST Requires:**
Policies, processes, and procedures are in place to address organizational risk and
to ensure that AI risk management is integrated into broader enterprise risk management.

**How to Implement:**

1. **Draft an AI Governance Policy** — use the template at
   [templates/ai-governance-policy.md](../templates/ai-governance-policy.md).
   Key elements:
   - Scope (which systems are covered)
   - Risk tolerance statements
   - Prohibited uses
   - Regulatory alignment (NIST AI RMF, EU AI Act, ISO 42001, industry-specific)

2. **Establish an AI Governance Committee** — minimum participants:
   - AI/ML Engineering Lead
   - Legal / Compliance representative
   - Privacy Officer (if applicable)
   - Business stakeholder for each high-risk AI system
   - CISO (for security-relevant AI systems)

3. **Define AI risk tolerance** — documented thresholds for:
   - Accuracy / performance minimums by risk tier
   - Maximum acceptable bias ratios
   - Acceptable latency and availability targets
   - Escalation triggers for governance review

**Checklist:**
- [ ] AI governance policy drafted and approved
- [ ] AI governance committee established with named members
- [ ] AI risk tolerance statements documented
- [ ] Policy aligned with applicable regulations
- [ ] Annual policy review process scheduled

---

### GV.2 — Roles and Responsibilities

**What NIST Requires:**
Accountability for AI risk management is clearly defined and documented throughout
the organization and its AI supply chain.

**How to Implement:**

Use this RACI model for AI governance:

| Activity | AI Lead | Legal | Security | Business Owner | AI Governance Committee |
|---|---|---|---|---|---|
| AI policy creation | C | R | C | I | A |
| Risk assessment | R | C | C | I | A |
| Model approval | R | C | C | A | R |
| Incident response | R | C | R | I | I |
| Regulatory reporting | I | R | C | I | A |
| Model retirement | R | I | I | A | I |

*R=Responsible, A=Accountable, C=Consulted, I=Informed*

**Checklist:**
- [ ] RACI matrix defined for all AI governance activities
- [ ] Named individuals assigned to each role
- [ ] Escalation paths documented
- [ ] Roles included in job descriptions and performance objectives

---

### GV.3 — Organizational Culture

**What NIST Requires:**
An organizational culture of responsible AI is cultivated, including training and
awareness programs, and the ability for personnel to raise AI risk concerns.

**How to Implement:**

1. **Training requirements by role:**
   - All AI practitioners: NIST AI RMF foundations (use [NIST's free materials](https://www.nist.gov/artificial-intelligence/ai-risk-management-framework))
   - AI leads: Bias evaluation, explainability techniques, incident response
   - Legal/compliance: Regulatory landscape (EU AI Act, ISO 42001)
   - Business owners: Risk tolerance decisions, governance escalation

2. **Speak-up mechanisms:**
   - Anonymous reporting channel for AI safety concerns
   - Regular retrospectives on AI system performance
   - Post-incident blameless reviews

3. **Recognition:**
   - Recognize and reward safety-positive behaviors
   - Include responsible AI in performance reviews for AI roles

**Checklist:**
- [ ] Training program defined by role
- [ ] Training completion tracked and documented
- [ ] Anonymous reporting mechanism in place
- [ ] Responsible AI included in performance evaluation criteria

---

### GV.6 — Model Inventory and Lifecycle Management

**What NIST Requires:**
AI risks and the overall AI risk management process are monitored and periodically
reviewed. AI systems are tracked across their lifecycle.

**How to Implement:**

Maintain a model inventory — see [templates/model-inventory.md](../templates/model-inventory.md).

Required fields for each model:
- System name and version
- Risk classification (high / medium / low)
- Business owner and technical owner
- Deployment date and environments
- Last governance review date
- Regulatory requirements applicable
- Retirement plan / end-of-life date

**Checklist:**
- [ ] Model inventory created and populated
- [ ] Quarterly review process established
- [ ] Ownership assigned for every production AI system
- [ ] Retirement / decommissioning process defined

---

## Templates for GOVERN Function

- [AI Governance Policy](../templates/ai-governance-policy.md)
- [Roles and Responsibilities RACI](../templates/raci-matrix.md)
- [Model Inventory](../templates/model-inventory.md)
- [Training Log](../templates/training-log.md)

---

## Next: [02 — MAP Function](02-map.md)
