# Plan & Progress — consciousleadershipcircle.in

A running record of what's shipped, what's in flight, and what's next.
Tick `[x]` as items land. Add new items as they appear.

Last reviewed: **May 2026**

---

## Shipped recently

### Site infrastructure
- [x] Verified end-to-end deploy pipeline (local → GitHub `main` → host → production); deploys land in ~15 seconds, both additions and deletions propagate cleanly
- [x] CLAUDE.md kept current as content lands (site structure, content inventory, mirror notes)

### Musings
- [x] **Can You Receive?** — Sree, on receiving as a capacity (already live before this session; CLAUDE.md updated to reflect it)
- [x] **Jo Hua So Hua** — Sree, on acceptance; published with **audio player (1m 55s MP3) + verbatim WhatsApp-forward transcript**; framed as a trusted friend forwarding the clip
- [x] **The MCA Question** — Sree, restructured chorus version of the sreebalakrishnan.in piece; **15 voice cards** in 6 themed clusters; prominent question card; "Still a Puzzle" section; **silent canonical** to sreebalakrishnan.in (matches mirror pattern)
- [x] **"The Two Whispers" hero illustration** added to The MCA Question; clickable lightbox; Open Graph image so the comic appears on LinkedIn/WhatsApp previews

### Articles (top-level)
- [x] **The Nine Presences** — Sree, the daśāvatāras mapped to leadership archetypes
  - [x] Multi-faith disclaimer at the top
  - [x] "Journey towards knowing myself" framing (replaces "Jyotish")
  - [x] 3×3 visual grid linking to 9 deep sections (anchor jumps)
  - [x] Krishna section visually differentiated (paper-deep background, Pūrṇa eyebrow)
  - [x] **English archetype label primary, Sanskrit name secondary** in cards and headings
  - [x] 9 universal/symbolic icons in `/images/avatars/*.png` (8 photoreal, Krishna watercolor)
  - [x] Krishna as `og:image` so the synthesis figure becomes the social card
  - [x] Self-canonical; small "If you want to go further" cross-link to the longer sibling essay on sreebalakrishnan.in/archetypes/

### Homepage / nav
- [x] Added **The Nine Presences** to homepage topbar nav (4 links now: The same question · The lotus · The nine presences · Musings)

---

## Open decisions — your call

- [ ] **Image style mismatch on Nine Presences.** Eight icons came back photoreal, Krishna came back watercolor. Three options on the table:
  - (a) Re-generate Krishna in photoreal style to match the eight
  - (b) Re-generate the eight in watercolor to match Krishna
  - (c) Ship as-is (the painted Krishna as the "integrated idea" while the eight are presences-in-the-world)
  - *Worth eyeballing the live grid before deciding*
- [ ] **Body-prose Sanskrit references on Nine Presences.** The synthesis and closing paragraphs still use the Sanskrit names verbatim (*"becomes Matsya for the new joinee, Kurma in the boardroom crisis..."*). Left intact for rhythm/brevity. Flip to English if you'd rather full consistency.
- [ ] **Reciprocal "tighter version" cross-link** on sreebalakrishnan.in/archetypes/ pointing back to CLC. Optional, nice symmetry — your task on the other repo.

---

## Verification still worth doing
- [ ] Open The Nine Presences on **mobile** — sanity-check the 3×3 grid wraps to 2 cols (≤700px) and 1 col (≤380px) without ugly cropping
- [ ] Paste both new article URLs into **LinkedIn Post Inspector** to confirm the og:image previews work (Krishna for Nine Presences, Two Whispers for MCA Question); LinkedIn caches aggressively
- [ ] Spot-check **one image crop per archetype** — the 1408×768 PNGs are center-cropped to square in the grid; any subject that got chopped is worth re-generating

---

## Backlog — pages yet to build (from CLAUDE.md)
- [ ] **`/reads/` or `/articles/`** — article index as the body of articles grows past 3–4. Currently top nav lists individual article names; that won't scale much further
- [ ] **Members-only page** — early access to trends, member profiles, dedicated content
- [ ] **Video podcast landing page** — member profiles + video, tied to the shared-corpus vision in CLAUDE.md

---

## Future musings / articles mentioned
- [ ] **A mentoring piece, co-authored with Siva** — surfaced during the Jo Hua So Hua reframe ("we should write about importance of mentoring — a topic close to you, we should do a podcast"). On the backlog
- [ ] **The Same Question** — already exists as a page but listed as "teased / in progress" in CLAUDE.md content inventory; may want a refresh pass
- [ ] **The Ancient Answer / The Lotus** — same status: page exists, may want a refresh pass

---

## Conventions worth keeping (lessons from this session)
- New musings → `/musings/<slug>.html`; link from `musings/index.html` above the `<!-- future musings -->` comment
- New top-level articles → `/<slug>.html`; link from homepage topbar nav
- Images for musings → `musings/images/`; for top-level articles → `/images/` (or `/images/<group>/` for sets)
- **Canonical = self by default.** Only point elsewhere if the *other URL has substantially the same text* — otherwise it's misleading
- **Mirror vs sibling vs syndication** are three distinct patterns. The Nine Presences taught us: don't assume "I'm publishing in two places" means "they're mirrors." Compare content before wiring canonical
- **Multi-faith framing**: when a piece draws from a specific tradition, an upfront disclaimer + universal English labels with cultural names as secondary works well. Don't strip the cultural specificity entirely — that erases the lineage and dulls the piece
- Every new page gets: canonical, Open Graph (`og:type`, `og:url`, `og:title`, `og:description`, `og:image` if there's an image), Twitter card, JSON-LD `Article`, Plausible analytics
- Footer "Last updated" should reflect when content last changed, not commit date
