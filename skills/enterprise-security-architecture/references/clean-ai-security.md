# Clean AI Security

Clean AI security checks AI-enabled software for security and privacy risks
without treating model output as trusted truth.

## Checks

- Is data classification known?
- Which prompts, tools, and models can access sensitive data?
- Can prompt injection or tool misuse cause harmful action?
- Are model outputs validated before business-critical use?
- Are secrets excluded from prompts and logs?
- Are tool permissions least privilege?
- Are audit logs sufficient and privacy-aware?
- Is human approval required for high-impact actions?
- Is fallback behavior defined?
- Is model or prompt versioning visible?

## Control Areas

- data minimization
- prompt and tool boundary
- output validation
- content and abuse monitoring
- human approval
- logging and auditability
- secrets handling
- model/prompt versioning
- incident response

Escalate evidence and acceptance decisions to `mournival-architecture` when AI
claims or AI-generated artifacts may become accepted architecture knowledge.
