# Security Policy

The Playbasis organization contains legacy repositories. Please report security issues privately and avoid publishing sensitive details before maintainers can respond.

## Reporting A Vulnerability

Use GitHub security advisories when available, or contact the maintainers directly.

Do not open public issues or pull requests containing:

- Live credentials or API keys.
- Webhook secrets or signing keys.
- Database dumps or customer data.
- Production hostnames that should not be public.
- Exploit steps that could put a live deployment at risk.

## Useful Reports

Useful reports include:

- Authentication or authorization bypasses.
- Tenant isolation failures.
- Public endpoint hardening issues.
- Insecure defaults or committed secrets.
- Callback, webhook, and integration validation problems.
- Unsafe file, content, notification, redemption, or reporting flows.

The June 2026 reset improved unsafe defaults and hardening in the canonical legacy stack, but this remains legacy infrastructure and should be reviewed carefully before deployment.
