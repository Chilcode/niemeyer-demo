> ## ▶ ACTIVE BUILD — read this first
>
> **Demo v2: fold in his real content.** The full spec is `.planning/HANDOFF.md`.
> Read it and `README.md` before editing.
>
> You own this repo. Do not write in `../realtor-chassis`, `../niemeyer`, or `../cch`.

**See `../context/PLAYBOOK.md` for cross-project conventions.**

# Michael Niemeyer — concept demo

A single self-contained HTML page. No build step, no dependencies, no external requests.
Published to GitHub Pages from `main` at https://chilcode.github.io/niemeyer-demo/.

Client context lives in `../niemeyer/CLAUDE.md`. Read it — it has his verified real data.

## Non-negotiables

This page pairs a **real, licensed** agent's name, phone number, and brokerage with
**invented listings**. Three things exist to keep that from becoming his problem:

1. `<meta name="robots" content="noindex, nofollow, …">` in the head
2. `robots.txt` disallowing all crawlers
3. The concept ribbon above the header

**Never remove any of them, and never make the sample listings look more real.** No
photographs, no plausible-looking MLS media. If it could be mistaken for his live site,
it's wrong.

## Deploy

Push to `main`. Pages rebuilds automatically. Verify after:

```bash
curl -s https://chilcode.github.io/niemeyer-demo/ | rg 'name="robots"'
```
