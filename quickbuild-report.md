# quickbuild report — Bonbino's

Built 2026-10-30 · 1 gate round(s) · **0 FAIL · 10 WARN**

## Warnings

- Inputs · Trust (E-E-A-T) inputs (site): Missing or thin: owner/founder names; opening year; 3+ real reviews with source; at least one social profile. Ask the client — never invent these.
- Inputs · Analytics configured (site): site.analytics.ga4Id is empty — the site will launch without traffic data
- Inputs · Featured items described (site): Every featured dish needs a menu description; signature items with no description waste the homepage's best slot
- Content · No repeated facts (/about/): Stated 4+ times: '$29.95' ×4 — say each fact once, where it's most useful
- Content · Lists joined once (/faq/): Double 'and' in a list: “…, meatballs and and extra cheese.”
- Content · No repeated facts (/faq/): Stated 4+ times: '10 am' ×6, '30 pm' ×4, '$29.95' ×11, '$20.50' ×4, '$14.50' ×5, '$10.50' ×6, '$9.50' ×5, '$20.95' ×5 — say each fact once, where it's most useful
- On-Page · No duplicate headings (/menu/): Repeated: eggplant rollatini, mussels marinara, chicken marsala
- Technical · No inline scripts (CSP) (/menu/): Inline <script> found; move it to a file so CSP can stay script-src 'self'
- Content · Word count ≥ 500 (/visit/): 448 words in <main>
- Content · Lists joined once (/visit/): Double 'and' in a list: “…, meatballs and and extra cheese.”

## Generic text in use (replace with the owner's words when you have them)

- `featured`
- `business.known_for`
- `business.story`

## Answers that would make the site stronger

- **/visit/** is 52 words short: answer visit.neighborhood_text, visit.landmarks, visit.parking, visit.transit in full
- `business.founding_year` — Year it opened (blank if unknown)
- `business.founding_date` — Exact opening date YYYY-MM-DD or YYYY-MM (blank if unknown)
- `business.description` — One factual sentence: what it is, where, since when
- `menu.dietary_note` — Dietary / allergy note that is TRUE (e.g. 'Gluten-free toast +$2; not a gluten-free kitchen.')
- `visit.arrival` — Best time to come / waits
- `visit.pickup` — Where to pick up online orders
- `amenities.wifi` — Free Wi-Fi?
- `amenities.high_chairs` — High chairs?
- `founders` — Owners / chefs
- `extra_faq` — Extra questions guests ask (optional)

## Next

- `npm run preview:bg` then open http://127.0.0.1:4321/ (stop with `npm run preview:stop`)
- Full gate: `npm run preview:bg && npm run check:full; npm run preview:stop`
- Deploy: see references/launch.md (Vercel, `VERCEL_DEEP_CLONE=true`)
