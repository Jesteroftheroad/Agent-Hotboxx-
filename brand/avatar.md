# HOTBOXX AI host — avatar lock record

**Status: LOCKED** (2026-09-24, concept 1A)

Once picked, change status to `LOCKED`, fill in the lock section, and never
change the face again.

## Concepts (Higgsfield Soul 2.0, 9:16)

| # | Name | Vibe | Job ID |
|---|---|---|---|
| 1 | **The Local Bhai** | Assamese guy, messy hair, stubble, huge grin, holding chicken dum biryani. Excited-friend energy — closest to the Scalio reference. | `03d1a211-c8dd-46e9-9524-785922a6fcde` |
| 2 | **The Hype Man** | Fade, gold chain, backwards cap, smirk, tandoori leg + tandoor flames. Edgy street energy — leans hardest into "Smoked. Fried. Certified." | `bd3ce8d1-f888-4820-a38c-f34ce4b905b1` |
| 3 | **The Foodie Nerd** | Curly hair, round glasses, laughing while tearing butter naan over butter masala. Relatable reviewer — best for rating/taste-test formats. | `feeca75b-344e-4d41-b10c-0c09d2ba6093` |

**Owner feedback (2026-09-24):** likes #1 Local Bhai, asked for versions built
from the owner's own reference photo (Higgsfield media `f0e65752-8a3b-4f1c-a2fe-330d7a2a87d3`;
the photo itself is not committed to the repo).

## Round 2 — reference face × Local Bhai look (GPT Image 2.5, 9:16)

| # | Variant | Job ID |
|---|---|---|
| 1A | Black tee, holding biryani, pointing, big grin (straight Local Bhai remake) | `686150dc-aeeb-4de5-9105-936f53122d88` |
| 1B | Leather jacket over black tee, tandoori plate, cheeky smile | `1baa8d3e-c64b-4bcf-b932-b5529bf17e52` |
| 1C | Chest-up, talking to camera, pointing at butter masala + roti | `27ac6456-8e2b-4343-9b5d-8e3a1c0c25f1` |

All round 1 concepts wear the black tee + dark warm-lit restaurant look from the Scalio
spec (`viral-formats.md` #13). They are view-only in the Higgsfield gallery
(Generations tab); this container can't download from Higgsfield's CDN.

## Lock plan (after the pick)
1. **Save as Reference Element** (instant, one image) — works directly with
   Kling 3.0 video, which is what we use for the reels. This is the primary lock.
2. Optional, for stills: generate 5–8 variations of the picked face (different
   angles/expressions, same outfit) and train a **Soul ID** on them (~10 min),
   used with Soul 2.0 for thumbnails/covers.

## Lock (fill in once picked)
- Picked concept: **1A** — owner's reference face × Local Bhai look (job `686150dc-aeeb-4de5-9105-936f53122d88`)
- Reference Element: `hotboxx-host` · ID `0f9872cf-3195-4591-ac86-287880991611`
  (use in Kling 3.0 / image prompts as `<<<0f9872cf-3195-4591-ac86-287880991611>>>`)
- Soul ID (optional): —
- Fixed wardrobe: plain black crew-neck t-shirt
- Fixed setting: dark restaurant interior, warm amber strip lighting
- Rules: presents dishes, delivers hooks, reacts. Never a fake customer, never a
  fake chef, never replaces real dish footage.
