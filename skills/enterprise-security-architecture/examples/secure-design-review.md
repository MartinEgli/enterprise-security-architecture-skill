# Example Secure Design Review

## Input

Review a new customer API exposed to partners.

## Output Shape

- Assets: customer data, partner credentials, audit logs
- Data classification: mark as gap if not supplied
- Trust boundaries: partner network, API gateway, internal services, data store
- Threats: credential abuse, data exfiltration, tampering, missing auditability
- Controls: OAuth/OIDC, mTLS where required, rate limits, schema validation,
  audit logging, secrets management, monitoring
- Residual risk: partner misuse and overprivileged access
- Approval: accepted with conditions or blocked if classification/identity is
  missing
