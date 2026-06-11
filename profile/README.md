# Playbasis

**Legacy gamification and rewards infrastructure, preserved for maintenance, documentation, and modernization.**

| Start Here | Status |
| --- | --- |
| [`playbasis/api`](https://github.com/playbasis/api) | Legacy runtime API for player actions, rules, rewards, quests, notifications, redemption, and reporting. |
| [`playbasis/control`](https://github.com/playbasis/control) | Legacy admin dashboard for configuring game mechanics, rewards, campaigns, players, reports, and integrations. |
| Website | [playbasis.ai](https://playbasis.ai) |
| Contact | [helloplaybasis@gmail.com](mailto:helloplaybasis@gmail.com) |

## Legacy Open Source Reset

> This is a legacy Playbasis application stack. The June 2026 work focused on preserving the existing system, improving compatibility, removing unsafe defaults, hardening public surfaces, and making the repositories usable again. It was not a feature-building push or a rewrite.

Playbasis is a legacy gamification and engagement stack. The public repositories contain historical business logic for player actions, rules, rewards, quests, quizzes, goods, notifications, reporting, SDKs, and an admin control plane.

The current open source reset is intentionally conservative: make the existing codebase easier to run, inspect, document, secure, and migrate from while preserving behavior.

## Canonical Repositories

- [`playbasis/api`](https://github.com/playbasis/api) - Legacy Playbasis gamification API for player actions, rules, rewards, quests, notifications, and redemption workflows.
- [`playbasis/control`](https://github.com/playbasis/control) - Legacy Playbasis admin dashboard for configuring game mechanics, rewards, campaigns, players, reports, and integrations.

Other public Playbasis repositories include SDKs, examples, documentation, or historical support code. Treat `api` and `control` as the canonical legacy application stack unless a repository states otherwise.

## What Is Here

- A legacy engagement engine for actions, points, rewards, badges, levels, campaigns, leaderboards, quests, and quizzes.
- A runtime API for player progress, event tracking, content, redemption, notification, social/integration callbacks, and reporting data.
- An admin console for configuring clients, sites, apps, rules, campaigns, rewards, goods, quests, quizzes, messages, widgets, users, reports, and integrations.
- SDKs and integration examples for older client stacks.
- Docker/runtime scaffolding and older Node support services.
- A reference implementation with substantial historical domain logic.

## What The Community Can Do Now

- Run the stack locally and improve setup documentation.
- Inspect the legacy domain model and document real behavior.
- Harden public endpoints, callbacks, tenant checks, and secret handling.
- Add regression tests around high-risk rules, rewards, redemption, and admin flows.
- Refresh SDK docs and mark stale demos clearly.
- Build adapters, API contract documentation, and migration helpers.
- Use the legacy stack as source material for a modern contract-first Playbasis Engine.

## Contribution Direction

Please prioritize preservation, compatibility, security, setup docs, tests, and migration support before feature expansion. This reset is about making useful legacy infrastructure maintainable again, not presenting it as a new SaaS launch.

See the [open source refresh strategy](../docs/open-source-refresh-strategy.md) for the current cleanup direction.
