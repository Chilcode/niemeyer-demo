# Prompt 04 — Demo v2: fold in his real content

**Run from:** `C:\Users\david.rios\Dev\niemeyer-demo`
**Model:** Sonnet.
**Isolation:** Separate repo. Safe to run alongside everything else.

---

## STOP. Re-ground first.
Read `README.md` in this repo and `../niemeyer/CLAUDE.md`. Open `index.html` and read it fully
before editing — it is one self-contained file, ~880 lines. Reply with a summary first.

## Context

This is a concept demo for Michael Niemeyer, live at https://chilcode.github.io/niemeyer-demo/
and already sent to him. It was built in ~20 minutes from public information during a phone
call, before we had his real content.

His actual site (https://michaelniemeyer.com/) has since given us better material. Your job is
to make v2 more *his* — not to redesign it.

## Your task

### 1. Fix what's wrong or missing
- **Office address** — currently absent. It is 2 Victory Dr, Liberty, MO 64068.
- **Email** — michael@therevolution1.com. Not shown anywhere.
- **Hours** — Daily 8AM–9PM. This is a real differentiator for a referral agent; show it.
- **2026 RealTrends Verified, top 1.5% nationwide.** Missing entirely, and it is his strongest
  credential. It belongs in the proof strip.
- The proof strip currently reads `100% By referral` — that is **our claim, not his**. Replace
  it with the RealTrends stat, which is verifiable.

### 2. Use his real voice
The current "How I Work" copy is invented. Replace it with his own, adapted from his site:
- *"Most agents unlock doors, write offers, and disappear between closings. That's not how I
  operate."*
- He was a **personal trainer** before real estate. His stated approach: *"listen first,
  educate without an agenda, and never push."* This is the best thing about his positioning
  and the demo doesn't mention it at all. Work it in properly — it explains *why* he operates
  the way he does.

### 3. Add the writing
He has three posts, and their headlines are his proof of expertise:
- "We Bought Our Home for $80,000. Nine Years Later, It Was Worth $214,000"
- "Your 3% Rate Feels Like an Asset. Here's When It's Actually a Trap"
- "What Does Waiting for Rates to Drop Actually Cost You in the Northland?"

Add a section. Headlines and a line of standfirst each — the point is to show the site has a
home for his thinking. If `../niemeyer/.planning/CONTENT.md` exists, pull real excerpts from it
rather than writing your own.

## Do NOT
- **Do not remove the demo ribbon, the `noindex` meta tags, or `robots.txt`.** They exist
  because this page pairs a licensed agent's real name with invented listings. Read the comment
  above the meta tags before touching that region.
- **Do not make the sample listings look more real.** They are fictional and must stay
  obviously labeled. Do not add photographs.
- Do not redesign. Navy + brass, Palatino display, monospace for data. If a section needs a new
  pattern, match the existing system.
- Do not add a framework, build step, or external request. One self-contained file, no
  dependencies, CSP-safe.
- Do not invent testimonials or quotes. He has 36 five-star Google reviews; we have the text of
  none of them.

## Definition of done
- Renders correctly in both light and dark (the page is token-driven; check both).
- No horizontal scroll at 375px width.
- `noindex`, `robots.txt`, and the ribbon all still present — verify after editing.
- Commit and push. Pages redeploys automatically from `main`.
- Confirm live: `curl -s https://chilcode.github.io/niemeyer-demo/ | rg 'name="robots"'`
