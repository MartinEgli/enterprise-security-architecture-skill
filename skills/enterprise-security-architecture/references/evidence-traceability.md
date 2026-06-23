# Evidence And Traceability

Use this reference whenever security findings, risks, controls, diagrams, or
approval recommendations depend on supplied inputs.

## Input Register

Track meaningful inputs by source type:

- User fact: stated directly by the user.
- Artifact: architecture diagram, policy, inventory, control list, data flow,
  risk register, code, or document supplied in the task.
- Tool result: command output, scan result, query result, validation result, or
  report.
- External source: cited standard, control catalog, regulation, documentation,
  or public reference.
- Assumption: useful but unverified working premise.

## Traceability Rules

- Preserve system names, asset names, trust boundaries, control IDs, data
  classifications, paths, and regulatory terms exactly.
- Tie each material risk and control recommendation to an input, source, or
  assumption.
- Do not treat missing data classification, ownership, or trust boundary as
  evidence.
- Do not claim compliance or approval from inferred controls alone.
- Keep conflicts visible and require human security review for high-impact
  ambiguity.

## Evidence Receipt

For substantial outputs, include a compact receipt:

| Finding Or Control | Source/Input | Type | Confidence | Gap Or Follow-up |
| --- | --- | --- | --- | --- |

Use `not supplied` when the input is missing. Use `assumption` when proceeding
with a working premise.

## Verification Pattern

Follow the small-loop pattern:

1. Locate relevant assets, data, identities, boundaries, and policies.
2. Make the smallest scoped finding or control recommendation.
3. Verify the output against evidence, assumptions, risk level, and skill
   boundaries.

Avoid unrelated architecture redesign; hand it to the owning architecture skill.
