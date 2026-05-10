# Security Policy

Entangle is pre-release. Please do not treat the current runtime as production
security-reviewed software.

## Reporting

Email security reports to:

`security@entangle.run`

Include:

- affected repository and commit;
- reproduction steps;
- impact;
- relevant logs, events, traces, or signed-message evidence;
- whether credentials, tokens, private keys, or repository data are exposed.

Please give reasonable time to investigate before public disclosure.

## Current Security Posture

The runtime is designed around explicit authority boundaries: Host Authority,
runner identity, User Node identity, operator access, node runtime identity,
and git principal identity.

Production security hardening is still required, especially around real
provider credentials, multi-machine deployment, audit retention, backup and
restore, and release operations.
