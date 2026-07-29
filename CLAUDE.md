> ## ⛔ RETIRED — 2026-07-29
>
> This concept demo is **superseded**. Michael delivered his own specification (see
> `../niemeyer/context/`), and it corrects most of what this demo proposed: "King of the
> Northland" and all crown/territory language are banned, the palette is River Bluff rather
> than Royals blue-and-gold, and the site uses no IDX — so the sample-listing search here
> represents a feature that will never be built.
>
> **Do not update this demo.** The real build is `../niemeyer/.planning/prompts/05-build-site.md`.
>
> It stays live only because Michael may still have the link. Take it down once the real site
> ships. The `noindex` tags, `robots.txt`, and concept ribbon must stay until then — this page
> pairs a licensed agent's real name with invented listings.

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
