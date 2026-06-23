---
name: enterprise-security-architecture
description: >
  Enterprise Security Architecture skill for secure design review, threat and
  risk assessment, control mapping, Zero Trust target architecture, security
  patterns, data protection, identity and access architecture, cloud security,
  AI security architecture, Clean AI security controls, security governance,
  and security approval recommendations.
---

# Enterprise Security Architecture

## Purpose

Support security architecture work by identifying threats, risks, control gaps,
security design decisions, target security architecture, and approval
conditions.

## When to Use

Use when the user asks for:

- secure design review
- threat or misuse analysis
- security architecture target state
- control mapping
- Zero Trust architecture
- identity and access architecture
- data protection architecture
- cloud or platform security architecture
- AI security architecture or Clean AI controls
- security governance or approval recommendation
- security risk treatment

## Do Not Use When

Do not use for general Enterprise Architecture strategy, capability maps, or
business roadmap work unless security is the main concern. Use
`enterprise-architecture` for general EA work.

Do not use for code-level Clean Architecture, Clean Coding, API design, or DDD
modeling unless the question is specifically about security risk or controls.
Use `software-architecture` or `domain-driven-design` for those.

Do not use for final evidence acceptance, architecture gate approval, or
productive-use governance of AI-generated artifacts. Use
`mournival-architecture` for those.

## Mandatory Rules

- Start from asset, data, trust boundary, identity, threat, and business impact.
- Separate threat, vulnerability, risk, control, residual risk, and decision.
- Mark assumptions and missing evidence.
- Do not claim compliance, legal adequacy, or production approval without
  verified source and accountable human approval.
- Prefer defense-in-depth and least privilege.
- Preserve supplied system names, control IDs, data classifications, and
  regulatory terms exactly.
- If asset, data classification, trust boundary, or identity context is missing,
  mark the review as incomplete and state the security impact of the gap.
- Escalate critical risk and unclear data classification to human security
  review.
- Escalate non-security architecture strategy to `enterprise-architecture` and
  code or service design concerns to `software-architecture`.

## Inputs Expected

- system or architecture under review
- data classification
- identities and actors
- trust boundaries
- interfaces and integrations
- cloud/platform context
- known controls
- regulatory or policy constraints
- threat scenarios
- target deployment context
- AI model, prompt, agent, tool, or data flow context when AI is involved

## Modes

### /esa review

Review security architecture and produce findings, controls, residual risks,
and approval recommendation. Read `references/security-method.md`.

### /esa threat

Identify threats, misuse cases, trust boundaries, and attack paths. Read
`references/threat-model.md`.

### /esa controls

Map risks to preventive, detective, and corrective controls. Read
`references/control-mapping.md`.

### /esa target

Create target security architecture and transition recommendations. Read
`references/security-target.md`.

### /esa decision

Prepare security architecture decision recommendation and approval conditions.
Read `references/security-governance.md`.

### /esa clean-ai

Review AI-enabled systems for security, privacy, abuse, prompt/tool exposure,
data protection, logging, human control, and residual risk. Read
`references/clean-ai-security.md`.

## Evidence Handling

- Evidence: supplied architecture, policy, inventory, control, source, or user
  fact.
- Inference: reasoned conclusion from evidence.
- Assumption: useful but unverified.
- Gap: missing item that can change risk or approval.

## Output Contracts

Use `assets/templates/esa-output-template.md` unless user asks for another
format.

## Quality Gates

- Assets and data classification are explicit.
- Trust boundaries are visible.
- Threats and risks are separated.
- Controls map to risks.
- Residual risk is stated.
- Approval conditions are explicit.
- Human security review is required for high or critical risk.
- AI-enabled systems define model, prompt, tool, data, logging, fallback, and
  human-control boundaries.

## Boundaries

- Do not replace accountable CISO, security board, privacy, legal, or compliance
  approval.
- Do not provide exploit instructions.
- Do not invent policy, regulatory, or control evidence.
- Do not approve production use with unresolved high or critical risk.

## Output Style

- Structured and risk-oriented.
- Use concise findings.
- Prefer tables for threat/control mapping.
- Use exact security terms and control IDs when supplied.
