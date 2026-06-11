# Contributing To Playbasis

Playbasis public repositories are mostly legacy infrastructure. Contributions should prioritize preservation, compatibility, security, setup documentation, tests, and migration support over new feature expansion.

## Preferred Contributions

- Documentation that clarifies real legacy behavior.
- Compatibility fixes that preserve existing contracts.
- Security hardening for public endpoints, callbacks, tenant checks, and secret handling.
- Setup, Docker, and verification improvements.
- Regression tests around rules, rewards, redemption, players, reports, and admin workflows.
- SDK compatibility notes and migration/adaptation helpers.

## Pull Request Expectations

Please include:

- What behavior should remain unchanged.
- Verification commands and output.
- Config, environment variable, secret, migration, or deployment impact.
- Any legacy compatibility assumptions.

Do not include live credentials, customer data, database dumps, private hostnames, or production secrets.
