# kinetwin-legal (STAGING, NOT PUBLISHED)

This is a staging README. Replace it with the neutral public README before the first push (see the publish commands). Do not push this file.

Source for a GitHub Pages site (Jekyll, theme `minima`) that will be served at https://smasher4459.github.io/kinetwin-legal/ . It holds the privacy notice and participant information for the Kinetwin TestFlight beta. No analytics, no third-party scripts, no externally hosted fonts.

## Files

| File | What | Source |
|---|---|---|
| `index.md` | Landing page: one line on Kinetwin, links to the two texts | written here |
| `privacy.md` | Privacy notice `beta-notice-v2` at `/privacy/` | `privacy-notice_v2.md`, body copied unchanged under a Jekyll front matter block |
| `beta.md` | Participant information `beta-sheet-v2` at `/beta/` | `beta-participant-sheet_v2.md`, body copied unchanged under a Jekyll front matter block |
| `_config.yml` | Theme `minima`, no analytics keys, README excluded from the site | written here |

The sources are in the private workspace at `~/formlab/_master/legal/beta/`. To change a text, change it there and re-copy; do not edit the body here.

## The `{{CONTACT_EMAIL}}` placeholder

`{{CONTACT_EMAIL}}` stood for the dedicated contact address. On 2026-10-28 it was replaced everywhere with kinetwin@proton.me (decision 1); this section is kept for history. It appears in `index.md`, `privacy.md` and `beta.md`.

Replace it in those three files before publishing, and use the same address as the TestFlight Feedback Email. Do not publish with it still in place: Jekyll reads `{{ ... }}` as a Liquid variable and renders an unknown one as an empty string, so the live page would silently have no contact address.

## Launch checklist

`~/formlab/_master/legal/beta/launch_checklist.md` (internal, not part of this repo). Nothing is pushed or published until every box in its "Launch checklist" is ticked, in particular section A (accounts, contact address, this repo) and section D (day of publishing: replace the placeholder, update the date at the top of both texts if publishing after 2026-10-28, check every link).

## Versions

When a new version of a text is published, first copy the current page to a file that keeps the old version reachable (for example `privacy-beta-notice-v2.md` with `permalink: /privacy/beta-notice-v2/`), then update `privacy.md`. The notice promises that earlier versions stay available.
