# Security Architecture Diagrams

Use this reference for `/esa diagram` or when the user asks for a security
architecture diagram.

## Scope

Create diagrams only for security architecture concerns:

- trust boundary diagrams
- data flow diagrams with classification
- identity and access flows
- threat paths and misuse paths
- control maps and defense-in-depth views
- Zero Trust policy decision/enforcement views
- cloud security topology at architecture level
- AI security flows: model, prompt, tool, data, logging, fallback, and human
  control

Hand general capability, roadmap, or portfolio diagrams to
`enterprise-architecture`. Hand code-level component, class, or detailed runtime
sequence diagrams to `software-architecture`.

## Notation Choice

- Mermaid `flowchart` for trust boundaries, control maps, and data flows.
- Mermaid `sequenceDiagram` for identity, token, approval, or tool-call flows.
- PlantUML component/deployment/sequence diagrams for security diagrams that
  need stable architecture-as-code.
- Use simple DFD-style labels when helpful: external actor, process, data store,
  trust boundary, data flow.

## Diagram Rules

- Mark trust boundaries explicitly.
- Label identities, actors, data classification, control points, and residual
  risk where known.
- Do not provide exploit instructions, payloads, bypass steps, or procedural
  attack guidance.
- Do not claim compliance or approval from a diagram alone.
- Mark assumptions and gaps that change risk.

## Output Pattern

1. State security purpose and assets in scope.
2. State notation used and why.
3. Provide diagram code.
4. List threats, controls, residual risks, and approval conditions.
5. Identify human security review triggers.
