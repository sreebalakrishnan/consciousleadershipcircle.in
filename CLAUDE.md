# consciousleadershipcircle.in — Project Memory

## What this site is

A web presence for the **Conscious Leadership Circle (CLC)** — a community of technology leaders navigating the pace of AI with clarity, groundedness, and each other. Not a course, not a framework. A Sangha: a trusted circle where leaders can be real, not perform.

Started as a thought. Then an in-person session across a few cities in India. Now slowly finding its rhythm.

---

## Founding members

| Name | Role | LinkedIn |
|---|---|---|
| Sunil Rawlani | Mentor · Co-founder | https://www.linkedin.com/in/rawlani/ |
| Siva | Co-founder | https://www.linkedin.com/in/sivaramasundar/ |
| Roopa | Co-founder | https://www.linkedin.com/in/roopasreeranganna/ |
| Santosh | Co-founder | https://www.linkedin.com/in/santosh-a-14954062/ |
| Sree Balakrishnan | Co-founder · Maintains site | https://www.linkedin.com/in/sreekandhbalakrishnan/ |

**WhatsApp contacts:**
- Sree: +919880330330
- Sunil: +919820331113

---

## Site structure

```
/                             → index.html                          Homepage (CLC hub — who we are, how we gather, founding members)
/the-same-question            → the-same-question.html              Article: Luddite comic, gate, founding story, Sunil's pillars
/lotus                        → lotus.html                          Article: Buddhism, Taoism, Stoicism, Gita — four traditions
/the-nine-presences           → the-nine-presences.html             Article: Sree — eight workplace archetypes (daśāvatāras) + Krishna as the Pūrṇa; 3×3 visual grid; icons at /images/avatars/{matsya,kurma,varaha,narasimha,vamana,parashurama,rama,balarama,krishna}.png
/musings/                     → musings/index.html                  Musings index — listing of all community reflections
/musings/a-day-with-ram-charan → musings/a-day-with-ram-charan.html  Musing: Vikas Anand — five take-aways from a one-day workshop with a popular leadership coach (three leader traits · the salesperson's gift · right people in right jobs · inside-out vs outside-in future-back goal-setting · personal growth as the lever for excellence). **Public framing keeps the coach anonymous** ("a popular leadership coach", "he"); internal note: the workshop was Dr. Ram Charan's, but Sree chose not to name him on the page. Opens with a small `.about-author` block: *Vikas is a Senior Director of Engineering at Yubi; ~two decades across CredAvenue, Mettl, Dell, Oracle.* (Earlier draft also mentioned IIT Kharagpur / "trained as a mathematician"; removed at Vikas's request.) Lightly polished but kept in Vikas's voice; opens with a short editorial note that the points/structure are his. Closes with his actual sign-off ("Hopefully it would be relevant to the leaders") in a `.signoff` block, followed by a `.signoff.reader-q` callout asking the circle: *"Knowing is one part of learning. Integrating what you know is the other part — often the harder one. How do you integrate the knowledge you acquire?"* (moss left-border to differentiate it from Vikas's sign-off). No named reading list — removed when the page was made anonymous. URL slug retains `ram-charan` for now (the page just shipped; renaming would 404 any links already shared). Uses the `.practice` block pattern from `what-the-system-sees.html` for each take-away
/musings/indian-voices-on-the-inner-mind → musings/indian-voices-on-the-inner-mind.html Musing: Sree (full curation) — sister piece to fifteen-psychologists. Fifteen Indian voices (Vyāsa, Vālmīki, Buddha, Mahāvīra, Kṛṣṇa, Patañjali, Nāgārjuna, Śaṅkara, Kabīr, Ramakrishna, Vivekānanda, Aurobindo, Ramaṇa, Krishnamurti, Nisargadatta) with dates + tradition + one-liner + Sanskrit key concept; six highlighted as "most relevant to modern conscious leadership"; Sree's personal reflection + "Did you know" aside on the 1880–1950 Indian renaissance cluster + Amazon.in reading list. Lines are Sree's distillations (not verbatim quotes — except Vivekānanda and Krishnamurti). Uses .curated/.voice-list classes (parallel to .forward/.psych-list on sister page)
/musings/fifteen-psychologists → musings/fifteen-psychologists.html Musing: Sree (light frame) — fifteen Western psychologists, one-line summary each from a LinkedIn forward (author unknown). Has grown well beyond the original frame: each entry now carries dates · country + a key-field tag with 6 highlighted as "most cited in modern knowledge work" (Jung, Maslow, Bandura, Festinger, Kahneman, Seligman); two prose paragraphs acknowledge the Western lens and point to Indian traditions (cross-link to /lotus.html + live link to the sister musing); a "Did you know" aside on the Nazi-era Vienna/Berlin → America displacement (Freud, Adler, Erikson, Horney, Fromm + Kahneman as child); an "If you want to go deeper" reading list with 15 Amazon.in search links. Uses .forward block (paper-deep box, "Forwarded · author unknown" label) because the list itself is verbatim third-party content
/musings/can-you-receive      → musings/can-you-receive.html        Musing: Sree — receiving as a capacity, the asymmetry of giving vs. receiving
/musings/jo-hua-so-hua        → musings/jo-hua-so-hua.html          Musing: Sree — acceptance as the floor under peace and happiness; verbatim WhatsApp forward (author unknown)
/musings/the-mca-question     → musings/the-mca-question.html       Musing: Sree — should a BCA grad do an MCA? Mirror of sreebalakrishnan.in piece, canonical points there
/musings/what-the-system-sees → musings/what-the-system-sees.html  Musing: Siva — "Curve-Balled by the System": annual review, leverage points, 3 practices
/what-the-system-sees         → what-the-system-sees.html           Redirect → /musings/what-the-system-sees.html
/puzzle                       → puzzle.html                         Dormant redirect to / — do not edit for content
/origins                      → origins.html                        Dormant — superseded by the-same-question.html
```

> **Important:** Edit `index.html` directly for homepage changes. `puzzle.html` and `origins.html` are dormant legacy files.
> When adding a new musing: create `musings/[slug].html`, add an entry to `musings/index.html` above the `<!-- future musings -->` comment.

### Pages yet to build
- `/reads/` or `/articles/` — article index as content grows
- Members-only page (early access to trends)
- Video podcast landing page (member profiles + video)

---

## Design system

Both pages share one design system. Do not introduce new fonts or colors without updating both.

### Colors
```css
--paper:      #FBFBF8   /* page background */
--paper-deep: #F4F2EB   /* section contrast, card backgrounds */
--ink:        #14181D   /* primary text */
--ink-soft:   #4B5560   /* body text, secondary content */
--ink-faint:  #8B95A0   /* labels, timestamps, meta */
--moss:       #3F5847   /* primary accent — links, borders, highlights */
--moss-soft:  #6E8473   /* secondary moss — member LinkedIn links */
--indigo:     #3D4F7C   /* used in lotus block (Stoicism tradition) */
--rule:       #E5E2DA   /* borders */
--rule-soft:  #EEEBE2   /* subtle dividers */
```

### Typography
```css
--display: "Bricolage Grotesque"   /* headings, labels, UI */
--serif:   "Instrument Serif"      /* pull quotes, italics, literary moments */
--sans:    "Inter Tight"           /* body text, navigation, captions */
```
Noto Sans Devanagari is loaded on origins.html only (for Sanskrit callouts).

### Shell widths
- Homepage (index/puzzle): `max-width: 720px`
- Origins: `max-width: 640px`
- The Lotus: `max-width: 680px`

---

## Tone guide

- **Voice:** warm, unhurried, precise. Not corporate. Not self-help.
- **Pronouns:** first person plural ("we", "us", "the circle") for the community; first person singular ("I") when Sree is clearly the author.
- **Sanskrit words:** used intentionally — Sangha, Chetana, Abhaya, Dharma. Always explained in context. Never decorative.
- **Attribution:** Sunil Rawlani is credited by name for the four pillars. Always.
- **No name-dropping for credibility.** Ideas stand on their own. If an external reference is used, it must be grounded in lived experience.
- **No corporate language:** avoid "pre-negotiated vulnerability contract", "framework", "methodology", "deliverable".

### The four pillars (Sunil Rawlani)
These are the anchor of the circle. Always rendered consistently:
1. Lead from authenticity — step beyond the job script.
2. Stay connected to your inner calling — your personal why.
3. Invest in inner transformation — stop running on old programming.
4. Build a Sangha — a trusted circle where leaders can be real, not perform.

---

## Content inventory

### Articles live
- **The Architecture of Courage** — on Abhaya, The Witness, The word before the storm. By Sree. Full version on Substack: https://sreebalakrishnan.substack.com/p/the-architecture-of-courage
- **The Nine Presences** — eight workplace archetypes (daśāvatāras) every team carries + Krishna as the Pūrṇa Avatāra to integrate into. 3×3 visual grid linking to nine deep sections, with per-archetype universal/symbolic icons (mostly photoreal; Krishna is watercolor) in `/images/avatars/*.png`. Multi-faith disclaimer at the top; English archetype label primary, Sanskrit name secondary. By Sree Balakrishnan. `/the-nine-presences.html`. Self-canonical. A *sibling* piece — not a mirror — to the longer essay "The Nine Masks at the Table" on sreebalakrishnan.in/archetypes/ (~6,700 words, with sections on "what an avatāra actually is" and "why Kṛṣṇa is the ninth"); a small "If you want to go further" block at the end of the closing section links to it.

### Musings live
- **A day with a leadership coach** — five take-aways from a one-day company-sponsored workshop with a "popular leadership coach": the three characteristics of a high-performing leader (clarity, visualisation + accountability, creating interest), the best salesperson's single gift (understanding the customer's needs), keeping the right people in the right jobs (job content, KPIs, training, accountability + follow-through), goal-setting from the future back vs the rear-view, and personal growth as the lever for people to excel. Lightly polished but Vikas's structure and voice throughout; closes with his actual sign-off line + a question-to-the-circle callout on knowing vs integrating knowledge. By Vikas Anand. `/musings/a-day-with-ram-charan.html`. *Internal note: the coach was Dr. Ram Charan; page deliberately keeps him anonymous.*
- **Curve-Balled by the System** — annual review blindside, leverage points (Donella Meadows), three practices of a conscious leader. By Sivarama Sundar. `/musings/what-the-system-sees.html` (redirect at `/what-the-system-sees.html`)
- **Can You Receive?** — receiving as a capacity, not a skill; the asymmetry of giving vs. receiving and what it means for how we lead. By Sree Balakrishnan. `/musings/can-you-receive.html`
- **Jo Hua So Hua** — on acceptance as the floor under peace and happiness; framed around a mentor's grounding and a verbatim WhatsApp forward (author unknown). By Sree Balakrishnan. `/musings/jo-hua-so-hua.html`
- **The MCA Question** — should a fresh BCA grad spend ₹5–6 lakh on an MCA, or start working first? A real question from a family + the chorus of responses from a circle of tech leaders. By Sree Balakrishnan. `/musings/the-mca-question.html` (mirror of `sreebalakrishnan.in/inklings/2026-05-22-the-mca-question.html`; canonical points there, silent — no visible "first published" banner)
- **Fifteen psychologists, one line each** — a LinkedIn forward (author unknown): fifteen Western psychologists, one-line summary each. Iterated significantly past the original frame: each entry carries *dates · country* and a *key-field* tag (6 highlighted as most cited in modern knowledge work — Jung, Maslow, Bandura, Festinger, Kahneman, Seligman); a "Did you know" aside flags the Nazi-era Vienna/Berlin → America displacement that shaped mid-century American psychology; an "If you want to go deeper" reading list links 15 Amazon.in searches (one starter book per author). Two prose paragraphs in Sree's voice acknowledge that the list is a Western cut and point to Indian traditions + the sister musing. `/musings/fifteen-psychologists.html`
- **Indian voices on the inner mind, one line each** — sister to *Fifteen psychologists*. Fifteen Indian voices spanning ~2,500 years (Vyāsa through Nisargadatta), each with dates · tradition + Sanskrit key concept + a one-line distillation. Sree's curation (not a forward) — the page is transparent that the lines are distillations, not quotes, except Vivekānanda's and Krishnamurti's. Six highlighted as *"most relevant to modern conscious leadership"* (Buddha, Kṛṣṇa, Patañjali, Śaṅkara, Ramaṇa, Krishnamurti). "Did you know" aside flags the 1880–1950 Indian renaissance cluster — six of the fifteen alive in one overlapping window. Reading list: 15 Amazon.in searches (Bibek Debroy's Mahābhārata/Rāmāyaṇa, Easwaran's Gītā/Dhammapada, Bryant's Yoga Sūtras, Godman's *Be As You Are*, Krishnamurti's *Freedom from the Known*, etc.). Uses `.curated`/`.voice-list` class names (semantically parallel to `.forward`/`.psych-list` on sister page; same visual treatment). Cross-links to *Fifteen psychologists* in the topbar and lede. `/musings/indian-voices-on-the-inner-mind.html`

### Articles teased / in progress
- **The Same Question** — the Luddite comic and founding story (`the-same-question.html`)
- **The Ancient Answer** — Buddhism, Taoism, Stoicism, Gita — four traditions (`lotus.html`)

---

## Gate / passcode (origins.html)

The origins page has a passcode gate — a Luddite comic puzzle. Any of these words unlock it:
`pause, breathe, chetana, sangha, lotus, human, witness, presence, reflect, dharma, aware, awareness, luddite, thrive, inner, equanimity`

The hint text: "Think about what this community is — or what the practice asks of you first."

---

## Shared corpus

Voluntary contribution model. Suggested anchor: ₹1,000 (cost of coffee for two at Starbucks). No fixed obligation. All contributions transparent and published on the page. Contact Sree on WhatsApp to discuss.

### Vision for the corpus
- Video podcast — member profiles, ideas, voice
- Co-authored articles
- Members-only page — early access to trends
- In-person retreats and session materials

---

## Footer standard (all pages)

```
[Site name] · consciousleadershipcircle.in     Maintained by Sree Balakrishnan
Started as a thought. Then an in-person session across a few cities in India. Now slowly finding its rhythm.
Created [Month Year] · Last updated [Month Year]
```

When adding a new page, update "Last updated" on all pages.

---

## Key decisions log

| Date | Decision |
|---|---|
| May 2026 | Moved from sreebalakrishnan.in subpage to standalone domain |
| May 2026 | Design system: adopted puzzle.html palette (moss, cool paper) across all pages |
| May 2026 | puzzle.html → new index.html (homepage); old index → origins.html |
| May 2026 | Philosophical section (Gita/Stoicism) extracted to the-lotus.html |
| May 2026 | All pages made Google-indexable (removed noindex) |
| May 2026 | Contribution model: removed fixed ₹1,000/session; voluntary with ₹1,000 as soft anchor |
| May 2026 | Architecture of Courage rewritten — removed Sinek attribution, "vulnerability contract", "8 minutes" |
