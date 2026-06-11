# Open Source Refresh Strategy

This strategy keeps the public Playbasis GitHub presence candid and useful. The organization contains a legacy app stack, SDKs, demos, and historical support repositories. The cleanup should make that structure obvious without overstating current product readiness.

## Current Public Position

- `playbasis/api` and `playbasis/control` are the canonical legacy application stack.
- The June 2026 reset focused on preservation, compatibility, unsafe-default cleanup, public-surface hardening, and usability.
- The reset was not a feature launch, a rewrite, or a claim that the historical stack is a polished new SaaS product.
- Older SDKs and demos should be labeled by status before they are promoted.

## Repository Tiers

### Tier 1: Canonical Legacy Stack

These repos should stay prominent and receive the most maintenance:

- `api`
- `control`

Expected public state:

- Current README with legacy banner.
- `docs/what-is-here.md`
- `docs/use-cases.md`
- `docs/maintenance-log-2026-06.md`
- `CONTRIBUTING.md`
- `SECURITY.md`
- PR template.
- Accurate repo description and topics.
- Release titled `June 2026 Legacy Maintenance Reset`.

### Tier 2: SDKs And Integration Libraries

These repos can help people understand how clients connected to the legacy API, but each one needs a status pass before promotion:

- `sdk`
- `sdk-php`
- `sdk-java`
- `sdk-python`
- `sdk-ruby`
- `sdk-ios`
- `sdk-android`
- `sdk-wordpress`
- `sdk-magento`
- `sdk-sharepoint`
- `sdk-pblib.js`
- `sdk-pblib.NET`
- `native-sdk-js`
- `native-sdk-ios`
- `native-sdk-android`
- `mobile-sdk-android`

Expected cleanup:

- Add a small legacy banner to each README.
- State whether it targets the legacy API or a historical deployment.
- Add topics such as `playbasis`, `sdk`, `gamification`, and the implementation language.
- Archive or label repos that cannot be built or verified.
- Avoid directing new production users to stale SDKs without compatibility notes.

### Tier 3: Demos, Widgets, Games, And Historical Samples

These repos can be useful examples, but they should not look like active production products:

- `html5game-sdk`
- `spinwheel-js`
- `spinwheel-ng2`
- `UnityNativePrototype`
- public demo or sample repos discovered during review.

Expected cleanup:

- Add a clear historical/demo banner.
- Explain which Playbasis primitive the demo illustrates.
- Add topics only after confirming the code content.
- Archive demos that no longer build or depend on private services.

### Tier 4: Documentation And Developer Portals

These repos need a content audit before being promoted:

- `Documentation`
- `developer`
- `developerplaybasis`, if made public in the future.

Expected cleanup:

- Mark stale docs clearly.
- Link canonical docs back to `api` and `control`.
- Move still-useful material into current repo docs or an OpenAPI-first documentation repo.

### Tier 5: Forks, Client Work, And Private Historical Repos

Forks and client-specific repositories should not be promoted in the public profile. Public forks should be archived or hidden from the profile unless they are intentionally maintained.

Expected cleanup:

- Keep private client repos private.
- Archive public forks that are not maintained.
- Avoid adding topics or descriptions that make private or obsolete work look canonical.

## Metadata Rules

Use conservative descriptions:

- Prefer `Legacy Playbasis ...` over broad claims.
- Prefer concrete nouns: API, admin dashboard, SDK, demo, integration.
- Mention preservation, compatibility, and modernization reference when relevant.
- Do not use phrases like `modern gamification platform` unless a repo has current docs, tests, and deployment verification.

Recommended common topics:

- `playbasis`
- `gamification`
- `loyalty`
- `rewards`
- `legacy-modernization`
- `engagement-engine`

Add language/framework topics only when verified from the repository contents.

## Cleanup Sequence

1. Keep `api` and `control` current and merge docs/security PRs promptly.
2. Publish the organization profile and default community health files.
3. Audit public SDK repos in small batches by language.
4. Add legacy banners and compatibility notes to SDK READMEs.
5. Archive or mark stale demos after build/readme inspection.
6. Consolidate still-useful docs into canonical docs or an OpenAPI-first documentation repo.
7. Pin only the canonical stack and verified SDK/documentation repos.

## Near-Term Engineering Follow-Up

The next engineering fix remains Control `user/autocomplete` auth and tenant hardening. Keep that separate from organization metadata cleanup.
