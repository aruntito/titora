# Security Policy

## Scope

TITORA is primarily an architecture and documentation hub. Security issues may still affect repository contents, documentation, automation, links, workflows, or referenced infrastructure.

## Reporting a vulnerability

Do not publish sensitive vulnerability details in a public issue.

Use GitHub's private security reporting mechanism for this repository when available. If private reporting is unavailable, contact the repository maintainer through a private channel before disclosure.

Include:

- affected file, workflow, or component
- concise vulnerability description
- reproduction steps, if safe to provide
- potential impact
- known mitigation, if any

Do not include credentials, access tokens, personal data, or other secrets in the report.

## Security principles

- **Least privilege** — components should receive only the access they require.
- **Explicit trust boundaries** — document where data crosses system or privilege boundaries.
- **No secrets in repositories** — credentials belong in appropriate secret-management systems.
- **Auditable automation** — automated actions should have observable inputs and outcomes.
- **Fail safely** — failures should not silently produce destructive or irreversible outcomes.
- **Dependency minimization** — avoid unnecessary infrastructure and third-party dependencies.

## Supported state

Security documentation describes the ecosystem's intended practices. Individual implementation repositories remain responsible for their own dependency, runtime, deployment, authentication, and infrastructure security.
