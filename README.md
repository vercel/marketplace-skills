# Vercel Marketplace Skills

Vercel-maintained, pinned mirrors of agent skills that the Vercel Marketplace
serves for partner products. Each skill is authored by the partner and
**unmodified** from a specific upstream commit; Vercel controls which commit is
served and reviews updates.

## Why this exists

A Marketplace product's `agentSkills` used to point directly at a partner's own
repository — a live pointer to their default branch. A partner could change the
installed content at any time, with no review. Mirroring here lets Vercel serve
a reviewed, pinned copy that upstream cannot change without a PR to this repo.

## Contents

| Skill | Author | License | Source | Pin |
| --- | --- | --- | --- | --- |
| `skills/neon-postgres` | Neon | Apache-2.0 | [neondatabase/agent-skills](https://github.com/neondatabase/agent-skills) | `b47b8830` (2026-05-21) |

See [`NOTICE`](./NOTICE) for attribution. Skill content is unmodified from the
pinned commit.

### Pin rationale

`neon-postgres` is pinned to **2026-05-21**, the last version before Neon's
June 2026 expansion of its skills into a full backend platform (Functions,
Object Storage, AI Gateway, Auth), which also added routing that treats Vercel
as a frontend/CDN. This is the database-era skill from roughly six months ago.

The `neon` platform-overview skill is **intentionally not mirrored**: it was
created in June 2026 specifically as that backend-platform pitch and has no
earlier, database-only form.

> ⚠️ The exact pin date is provisional — to be confirmed against the version
> Vercel reviewed at Neon's Marketplace onboarding.

## Updating

Updates are deliberate and reviewed: re-vendor a skill from a chosen upstream
commit, update its row and `NOTICE`, and open a PR. Nothing auto-syncs upstream.
