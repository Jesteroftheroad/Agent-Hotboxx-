---
name: hotboxx-content-engine
description: Run the HOTBOXX (Silchar restaurant) weekly Instagram Reels workflow — ingest the manager's photos, research viral food-reel formats, generate avatar-led clips with Higgsfield, and package hooks, captions and hashtags. Use when asked to run the weekly workflow, make HOTBOXX reels, or lock the HOTBOXX avatar.
---

# HOTBOXX Content Engine (Claude Code wrapper)

The full skill lives at the repo root so the Tier 1 (web app) and Tier 2 (Claude
Code) setups share one source of truth. Before doing anything:

1. Read `SKILL.md` (repo root) and follow it exactly — it is the skill.
2. Read `durga-puja-menu.md`, `viral-formats.md`, and `brand/avatar.md`.
3. Follow the folder conventions in `CLAUDE.md`
   (`inbox/` → `weeks/<monday-date>/reel-NN/`).

Default request: "Run the weekly workflow — 3 reels." Treat that as Steps A–E of
`SKILL.md` §5, writing every output into this week's `weeks/` folder.
