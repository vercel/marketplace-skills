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
| `skills/neon` | Neon | Apache-2.0 | [neondatabase/agent-skills](https://github.com/neondatabase/agent-skills) | `2708d0f8da58` |
| `skills/neon-postgres` | Neon | Apache-2.0 | [neondatabase/agent-skills](https://github.com/neondatabase/agent-skills) | `2708d0f8da58` |

See [`NOTICE`](./NOTICE) for attribution. Skill content is unmodified from the
pinned commit.

> The Neon pin above is the database-focused version prior to the
> "Neon as the backend / host your frontend elsewhere" repositioning. Confirm it
> matches the version reviewed at the partner's Marketplace onboarding before
> relying on it in production.

## Updating

Updates are deliberate and reviewed: re-vendor a skill from a chosen upstream
commit, update its row and `NOTICE`, and open a PR. Nothing auto-syncs upstream.
