# Michael Niemeyer — site concept

A design concept prepared by [Chilcode Systems](https://chilcode.com) for Michael Niemeyer,
REALTOR® with RE/MAX Revolution, serving Missouri's Northland (Clay and Platte counties).

**This is not a live real estate website.** Nothing here is production.

## What it demonstrates

- A visual direction — navy and brass — built specifically for this agent's market and
  practice, not adapted from a template.
- A working home-search interface. The filters genuinely filter, so the interaction can be
  demonstrated in a conversation.
- The referral-side surfaces a By Referral Only practice actually needs: a trusted-vendor
  list shared by request rather than published, and proof framed around families served
  rather than lead volume.

## What is fake, and deliberately so

Every listing is invented. The addresses, prices, MLS numbers, and listing offices are
sample data written to look plausible for the Northland market. **None of it came from
Heartland MLS.**

The page is marked as a concept in three places — a ribbon above the header, a notice
beneath the search results, and the legal block in the footer.

## Why this repo is not indexed

`index.html` carries `noindex, nofollow` and `robots.txt` disallows all crawlers.

This is not optional. The page pairs a licensed agent's real name, phone number, and
brokerage with invented inventory. If it appeared in a search for him it could be mistaken
for his actual site, and advertising listings that do not exist under a licensee's name is
a compliance problem for *him*. Do not remove the meta tags.

## Real IDX

A production build would pull listings from Heartland MLS through
[MLS Grid](https://kcrar.com/kcrar-members/heartland-mls/data-feeds-and-vendor-inquiries/).
That requires the agent and his broker to sign the MLS Grid Master Data License Agreement
and Heartland to approve the feed — it cannot be arranged on his behalf.

Heartland's IDX rules also constrain the build: the IDX mark and disclaimer must appear on
every listing, the listing office must be attributed, the term "MLS" is restricted in
branding, and search and listing pages cannot change after compliance review without
re-approval.

## Stack

One self-contained HTML file. No build step, no dependencies, no external requests.
