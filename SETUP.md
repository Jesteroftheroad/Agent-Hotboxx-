# SETUP GUIDE — HOTBOXX Content Engine

## What you're building

A repeatable weekly system: manager's photos/videos + menu go in → trend-backed
Reels and captions come out. Two tiers — start with Tier 1, graduate when you
want automation.

## TIER 1 — Claude web app (no code, ~15 min setup, works today)

**You need:** a Claude account + Higgsfield account.

1. **Connect Higgsfield to Claude**
   - In Claude (web or desktop): Settings → Connectors → Add custom connector
   - Name: `Higgsfield`, URL: `https://mcp.higgsfield.ai/mcp`
   - Click Add → Connect → sign in with your Higgsfield account → Allow
   - Verify: ask "what's my Higgsfield credit balance?" — if it answers, you're live.

2. **Install the HOTBOXX skill**
   - In Claude: go to Skills → upload `SKILL.md` from this folder
     (or create a new Skill and paste its contents).
   - Invoke it any time by typing `/` and picking the HOTBOXX skill,
     or just paste `MASTER_PROMPT.md` into a fresh chat for the zero-setup version.

3. **Lock your AI host avatar (one-time, 5 min)**
   - In your first run, Claude proposes 3 avatar concepts for the HOTBOXX host —
     pick one.
   - Claude saves it via Higgsfield's Soul ID (character consistency), so the same
     face shows up in every reel. This is what makes content effortless: no filming
     yourself or staff, ever. The avatar presents; your real food photos carry the
     OG vibe.

4. **Weekly run (10 min of your time — upload + approve, nothing else)**
   - Dump the manager's new photos/videos into the chat.
   - Say: "Run the weekly workflow — 3 reels."
   - Claude researches trends, generates avatar-led clips via Higgsfield, writes
     hooks + captions. You review, add trending audio in Instagram, post.

**Cost:** Higgsfield credits are priced per model/duration/resolution — check
higgsfield.ai/pricing before you start; a weekly run of short food clips is
typically a few dollars a month. Claude subscription as usual.

## TIER 2 — Full autopilot with Claude Code (for later)

Adds automatic viral-reel scraping so trend research isn't manual.

1. Install Claude Code, add two MCPs:
   - Higgsfield: `https://mcp.higgsfield.ai/mcp`
   - Apify: `https://mcp.apify.com` (sign in with Apify account)
2. Drop `SKILL.md` + `viral-formats.md` into the project as the agent's instructions.
3. Schedule it: `claude --schedule "every Monday 9am"` style cron, or just run it
   manually each week.

**Cost:** Apify's free tier includes monthly credits — enough for a weekly
hashtag scan at this scale; check apify.com/pricing for current numbers.
Higgsfield as in Tier 1.

## Honest limits (validated, not marketing)

- No tool sees "ALL viral reels" — scraping samples hashtags/profiles and ranks by
  engagement. It's a strong signal, not omniscience.
- Instagram scraping lives in a gray area of IG's ToS. Read-only trend research
  is low-risk, but don't automate posting via scrapers — post manually or via
  Meta's official API.
- AI video is best at ANIMATING your real food photos (steam, pour, sizzle).
  Fully AI-invented dishes can look fake — always lead with the manager's real shots.
- Text accuracy: AI video models still garble on-screen text. That's why the
  system keeps all text OUT of generated clips — you overlay it in Instagram.

## Files in this folder

- `SKILL.md` — the installable skill (brain + brand + workflow)
- `MASTER_PROMPT.md` — one-shot prompt for any Claude chat, no setup
- `viral-formats.md` — 10 proven reel skeletons adapted for HOTBOXX
- `SETUP.md` — this file
