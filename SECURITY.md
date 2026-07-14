# Security Policy

MONACOPS publishes public reference architectures for secure Agentic AI Operating Systems. Security, privacy, human approval and auditability are core requirements of every architecture in this repository.

## Reporting Security Issues

If you believe this repository contains a security issue, please report it privately by contacting:

**contact@monacops.com**

Please do not open a public issue for suspected vulnerabilities, leaked secrets, confidential data or exploitable implementation details.

## Scope

This policy covers:

- Public documentation in this repository
- Reference architecture guidance
- Security, governance and observability frameworks
- Mermaid diagrams and examples

This repository does not contain production systems, client deployments, proprietary source code, secrets or credentials.

## Security Principles

- Apply security by design.
- Use least-privilege permissions for every agent and integration.
- Require human approval for sensitive actions.
- Keep all actions auditable.
- Preserve privacy and confidentiality.
- Define explicit failure handling.
- Prefer graceful degradation over unsafe automation.
- Monitor agent behavior continuously.

## Sensitive Content Rules

Do not submit:

- Secrets or credentials
- API keys, tokens or private keys
- Client names or client data
- Internal network details
- Production incident details not approved for publication
- Proprietary source code
- Unsupported security claims

## Human Approval Requirements

Architectures in this repository should require explicit human approval for:

- External communication sent on behalf of a business
- Financial actions
- Legal, compliance or contractual actions
- Record deletion or irreversible updates
- Production system changes
- Actions that affect client experience, safety or obligations

## Response Expectations

MONACOPS will review security reports as quickly as practical and may request additional information to validate the issue. Public documentation updates will avoid disclosing sensitive operational details.
