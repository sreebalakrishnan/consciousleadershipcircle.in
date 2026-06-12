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
/the-unhurried-craft          → the-unhurried-craft.html            Article: Sree — seven Japanese words (Ikigai, Kaizen, Hara Hachi Bu, Kintsugi, Wabi-Sabi, Shinrin-Yoku, Omoiyari) as correctives to the "go faster" AI-era default; sibling to /lotus; four "movements"; collapsible essences; text-only (no images)
/reads/                       → reads/index.html                    Reading index — listing of all top-level articles (newest first); mirrors the /musings/ index pattern. Includes the 4 on-site articles + Architecture of Courage as an external (Substack ↗) entry. The single nav home for articles ("Reading"); individual article links no longer appear in the topbar
/conversations/               → conversations/index.html            Conversations index — long-form video conversations with members of the circle
/conversations/roopa-sreeranganna → conversations/roopa-sreeranganna.html  Conversation: Sree with Roopa Sreeranganna — "The accidental leader" (43 min, May 2026). YouTube video ID: `a8ap2LJTSNk` (https://youtu.be/a8ap2LJTSNk). YouTube embed (16:9 iframe, youtube-nocookie), Sree's three-para framing, 17-chapter list with clickable timestamp links opening YouTube in a new tab, "Three things that stayed with me" section pulling three Roopa quotes, closing pull, guest card linking to her LinkedIn.
/conversations/tuhin-mohanta  → conversations/tuhin-mohanta.html       Conversation: Sree with Tuhin Mohanta — "The builder who bounces back" (52 min, May 2026). YouTube video ID: `IbhqHXLJYuY`. Same pattern as the Roopa page (embed, framing, chapters, pulls, guest card).
/conversations/sivarama-sundar → conversations/sivarama-sundar.html    Conversation: Sree with Sivarama Sundar — "Three decades, five machines" (**audio-only**, 1 hr 41 min, June 2026). First audio episode; a new page pattern: Paris Review-style **edited interview** (Sree's questions in `.q` serif-italic blocks, Siva's answers as body prose) structured into five era sections ("five machines": dual-floppy 8086 1992–95 · Clipper years 1995–99 · Delphi decade 1999–2009 · gray shades 2009–23 · the machine that talks back 2023–); era-grouped chapter list (`.chapter-era` headings) whose rows **seek the embedded player inline** via YouTube iframe postMessage (`enablejsapi=1`), with watch?v= links as fallback; two verbatim `.duet` exchanges (Prince of Persia/Super Mario; the ₹750 paycheck); three `.gloss` "For the younger reader" asides (Borland/Norton, NIIT, floppy/TSR); a dark animated **DOS screen card** (`.dos`) recreating the raindrops virus (CSS-only falling characters, respects prefers-reduced-motion); a `.coda` accepting Siva's proposal that the next episode adds Sesame's Maya as a third (non-human) voice; closing pull "Happy to leave any tiny breadcrumbs…"; guest card links his LinkedIn + his musing. **YouTube ID is a placeholder**: replace `YOUTUBE_VIDEO_ID_HERE` in the inline script at the bottom of the page once the audio is uploaded — the player and chapter seeking light up from that one constant. No og:image (audio; `twitter:card` is `summary`). Self-canonical.
/gatherings/                  → gatherings/index.html               Gatherings index — notes from the circle's actual meetings (in-person + virtual). A distinct content type from Musings (single-author) and Conversations (1:1 video). Index modelled on /conversations/ (mast "When the circle *gathers*"; item list with format · date · voice-count). Uses `.gathering-item` classes.
/gatherings/ai-vs-human-frontier → gatherings/ai-vs-human-frontier.html  Gathering: "Navigating the AI vs. Human frontier" — the circle's **first virtual gathering** (May 2026, 7 voices). A multi-voice session summary. Has: a 6-panel comic hero (lightbox + og:image) at `/gatherings/images/ai-vs-human-frontier.png` (1536×1024; the `CLC-may29` comic; page hides the figure via `onerror` if the file is ever missing); Sree's framing prose; a `.consensus` card ("not AI vs. human, but AI + human"); seven `.speaker` cards (Sree · Sunil Rawlani · Nagamahesh Pingali · Arun Kundu · Solasa Rajesh · Surya Pandey · Tuhin Mohanta) each with role + view; a Sunil pull-quote; five `.theme-item` blocks (human in the loop · workflow vs autonomy · ownership & accountability · growth needs guardrails [Nagamahesh + Rohit Thomas; 5 guardrail chips] · the economics); synthesis + closing pull ("The future isn't AI versus humans. It's humans *with* AI."); a `.recording` block linking the **members-only Google Drive recording directly** (https://drive.google.com/file/d/1xBi0mbCB60HLM7S9ax1YRIoKGcRhkcCT/view) with a WhatsApp-Sree fallback for access. Self-canonical.
/sparks/                      → sparks/index.html                   Sparks index — short, alive moments from the circle's group chat (a screenshot, a forward, a one-line reply) and the conversation each set off. A fourth content type, distinct from Musings (single-author), Conversations (1:1 video) and Gatherings (meeting notes). Index modelled on /gatherings/ (mast "When something *catches*"; item list with format · date · voice-count). Uses `.spark-item` classes.
/sparks/context-is-everything → sparks/context-is-everything.html   Spark: "Should I walk or *drive?*" — the circle's **first spark** (May 2026, 5 voices). Venkata Rajesh Solasa shared a Claude screenshot (someone asked an AI whether to walk or drive to a car wash 100m away; it said "Walk. It's a one-minute stroll."). The thread that followed — Abhiram J (clear prompting), Vikas Anand (clear communication as a leadership trait), Tuhin Mohanta (context-awareness), Vikas again (the Mahābhārata Aśvatthāmā half-truth → "Context is everything"), Vaskar Nag ("good to walk to collect your car") — is rebuilt on the page as **chat bubbles, not screenshots**: a dark CSS `.ai-card` recreating the Claude exchange (coral SVG asterisk mark, serif reply, "Opus 4.8 · High" footer) + a `.thread` recreating the WhatsApp exchange (`.bubble` messages, sender names in moss/indigo/moss-soft, timestamps, emoji `.reacts` chips, a `.reply-quote` strip on Vaskar's message). Sree's framing prose walks the small observation up into a leadership one; a `.gloss` aside explains the Aśvatthāmā story for readers new to it; closing pull "Context is everything." Author: Sree Balakrishnan. Self-canonical. **No phone numbers published** (WhatsApp showed members' numbers; kept off the page). No og:image (chat is rendered in HTML, not a raster) — `twitter:card` is `summary`.
/musings/                     → musings/index.html                  Musings index — listing of all community reflections
/musings/a-day-with-ram-charan → musings/a-day-with-ram-charan.html  Musing: Vikas Anand — five take-aways from a one-day workshop with a popular leadership coach (three leader traits · the salesperson's gift · right people in right jobs · inside-out vs outside-in future-back goal-setting · personal growth as the lever for excellence). **Public framing keeps the coach anonymous** ("a popular leadership coach", "he"); internal note: the workshop was Dr. Ram Charan's, but Sree chose not to name him on the page. Opens with a small `.about-author` block: *Vikas is a Senior Director of Engineering at Yubi; ~two decades across Yubi, Mettl, Dell, Oracle.* (Note: CredAvenue rebranded to Yubi, so the company list folds CredAvenue into Yubi. Earlier draft listed Yubi twice in the same sentence — current phrasing reads "including stints at Mettl, Dell and Oracle" to avoid the repeat.) (Earlier draft also mentioned IIT Kharagpur / "trained as a mathematician"; removed at Vikas's request.) Followed by a "Did you know" `.aside`: *Vikas ran his own company 2012–2018; Mettl was his biggest client during those years, and later he joined Mettl as an employee — "the client became the team."* Lightly polished but kept in Vikas's voice; opens with a short editorial note that the points/structure are his. Closes with his actual sign-off ("Hopefully it would be relevant to the leaders") in a `.signoff` block, followed by a `.signoff.reader-q` callout asking the circle: *"Knowing is one part of learning. Integrating what you know is the other part — often the harder one. How do you integrate the knowledge you acquire?"* (moss left-border to differentiate it from Vikas's sign-off). No named reading list — removed when the page was made anonymous. URL slug retains `ram-charan` for now (the page just shipped; renaming would 404 any links already shared). Uses the `.practice` block pattern from `what-the-system-sees.html` for each take-away
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
> When adding a new top-level article: create `<slug>.html`, then add an entry to `reads/index.html` above the `<!-- future reads added above this comment -->` comment. **Do NOT add the article's own title to the topbar nav** — articles live behind the single `Reading` link; `/reads/` is their discovery surface.
> When adding a new conversation: create `conversations/[slug].html` (model on `roopa-sreeranganna.html`), add an entry to `conversations/index.html` above the `<!-- future conversations -->` comment. Episode pages should include: YouTube embed (`youtube-nocookie.com/embed/` domain, 16:9 aspect-ratio, `loading="lazy"`), Sree's framing prose, a clickable chapter list (each row linking to `youtube.com/watch?v=ID&t=Xs` in a new tab), and 2–4 pulled guest quotes with a Sree gloss.
> When adding a new gathering: create `gatherings/[slug].html` (model on `ai-vs-human-frontier.html`), add an entry to `gatherings/index.html` above the `<!-- future gatherings -->` comment. Gathering pages are multi-voice session summaries — `.speaker` cards (name + role + view), `.theme-item` blocks for cross-cutting themes, a `.consensus` card for where the room converged, and an optional comic hero + members-only `.recording` block.
> When adding a new spark: create `sparks/[slug].html` (model on `context-is-everything.html`), add an entry to `sparks/index.html` above the `<!-- future sparks -->` comment. Sparks are short group-chat moments rebuilt **as chat bubbles, not screenshots** — a `.thread` of `.bubble` messages (sender names, timestamps, emoji `.reacts`, optional `.reply-quote`), an optional dark `.ai-card` if an AI exchange is part of it, Sree's light framing prose, an optional `.gloss` aside for any reference worth explaining, and a closing pull. **Never publish phone numbers** even though WhatsApp shows them.

### Nav convention (as of June 2026)
The site now has five content surfaces, each with its own index: **Reading** (`/reads/` — articles) · **Musings** (`/musings/`) · **Conversations** (`/conversations/`) · **Gatherings** (`/gatherings/`) · **Sparks** (`/sparks/`). The topbar right-nav lists these section indexes (dropping the current page's own section), in the canonical order Reading · Musings · Conversations · Gatherings · Sparks, and collapses on narrow screens into a CSS-only hamburger (`.nav-toggle` checkbox + `.nav-burger` label, media query at ≤640px). **Individual article/post titles are never in the nav** — they live in their section index. This replaced the old per-article nav, which didn't scale. Leaf pages keep a "← All <section>" back-link as their first nav item where helpful. (Older article leaf pages — `lotus.html`, `the-same-question.html`, `the-unhurried-craft.html` — still carry a minimal `Reading · Musings` nav without the hamburger; harmless, worth standardising next time they're touched.)

### Pages yet to build
- Members-only page (early access to trends)
- ~~Video podcast landing page~~ — shipped as `/conversations/` (first episode with Roopa, May 2026)

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
- **The Unhurried Craft** — seven Japanese words read as correctives to the AI-era "go faster" default: Ikigai (purpose), Kaizen + Hara Hachi Bu (practice), Kintsugi + Wabi-Sabi (repair & enough), Shinrin-Yoku + Omoiyari (the body & the other person). Structured in four "movements" with collapsible essences (first word open, rest behind Read-more toggles). Kanji shown alongside each romaji label, explained in context. Text-only — no images, text-only OG/Twitter `summary` card. By Sree Balakrishnan. `/the-unhurried-craft.html`. Self-canonical. Explicit *sister reading* cross-link to `/lotus.html` (same theme, four older traditions). Reuses the Lotus design verbatim but renames the block classes `.lotus*`→`.gloss*`.

### Musings live
- **A day with a leadership coach** — five take-aways from a one-day company-sponsored workshop with a "popular leadership coach": the three characteristics of a high-performing leader (clarity, visualisation + accountability, creating interest), the best salesperson's single gift (understanding the customer's needs), keeping the right people in the right jobs (job content, KPIs, training, accountability + follow-through), goal-setting from the future back vs the rear-view, and personal growth as the lever for people to excel. Lightly polished but Vikas's structure and voice throughout; closes with his actual sign-off line + a question-to-the-circle callout on knowing vs integrating knowledge. By Vikas Anand. `/musings/a-day-with-ram-charan.html`. *Internal note: the coach was Dr. Ram Charan; page deliberately keeps him anonymous.*
- **Curve-Balled by the System** — annual review blindside, leverage points (Donella Meadows), three practices of a conscious leader. By Sivarama Sundar. `/musings/what-the-system-sees.html` (redirect at `/what-the-system-sees.html`)
- **Can You Receive?** — receiving as a capacity, not a skill; the asymmetry of giving vs. receiving and what it means for how we lead. By Sree Balakrishnan. `/musings/can-you-receive.html`
- **Jo Hua So Hua** — on acceptance as the floor under peace and happiness; framed around a mentor's grounding and a verbatim WhatsApp forward (author unknown). By Sree Balakrishnan. `/musings/jo-hua-so-hua.html`
- **The MCA Question** — should a fresh BCA grad spend ₹5–6 lakh on an MCA, or start working first? A real question from a family + the chorus of responses from a circle of tech leaders. By Sree Balakrishnan. `/musings/the-mca-question.html` (mirror of `sreebalakrishnan.in/inklings/2026-05-22-the-mca-question.html`; canonical points there, silent — no visible "first published" banner)
- **Fifteen psychologists, one line each** — a LinkedIn forward (author unknown): fifteen Western psychologists, one-line summary each. Iterated significantly past the original frame: each entry carries *dates · country* and a *key-field* tag (6 highlighted as most cited in modern knowledge work — Jung, Maslow, Bandura, Festinger, Kahneman, Seligman); a "Did you know" aside flags the Nazi-era Vienna/Berlin → America displacement that shaped mid-century American psychology; an "If you want to go deeper" reading list links 15 Amazon.in searches (one starter book per author). Two prose paragraphs in Sree's voice acknowledge that the list is a Western cut and point to Indian traditions + the sister musing. `/musings/fifteen-psychologists.html`
- **Indian voices on the inner mind, one line each** — sister to *Fifteen psychologists*. Fifteen Indian voices spanning ~2,500 years (Vyāsa through Nisargadatta), each with dates · tradition + Sanskrit key concept + a one-line distillation. Sree's curation (not a forward) — the page is transparent that the lines are distillations, not quotes, except Vivekānanda's and Krishnamurti's. Six highlighted as *"most relevant to modern conscious leadership"* (Buddha, Kṛṣṇa, Patañjali, Śaṅkara, Ramaṇa, Krishnamurti). "Did you know" aside flags the 1880–1950 Indian renaissance cluster — six of the fifteen alive in one overlapping window. Reading list: 15 Amazon.in searches (Bibek Debroy's Mahābhārata/Rāmāyaṇa, Easwaran's Gītā/Dhammapada, Bryant's Yoga Sūtras, Godman's *Be As You Are*, Krishnamurti's *Freedom from the Known*, etc.). Uses `.curated`/`.voice-list` class names (semantically parallel to `.forward`/`.psych-list` on sister page; same visual treatment). Cross-links to *Fifteen psychologists* in the topbar and lede. `/musings/indian-voices-on-the-inner-mind.html`

### Conversations live
- **The accidental leader — Roopa Sreeranganna** — first episode in the long-form video conversation series. Sree with Roopa (co-founder of CLC, 26 years in tech). 43 minutes. Themes: boundaryless thinking as risk preparation, the floor that a father's quiet promise builds under a daughter's courage, AI as an inflection point where the "soft" skills become *the* skills. Page has YouTube embed (iframe, youtube-nocookie, 16:9), Sree's three-paragraph framing, 17 clickable chapter timestamps, three pulled Roopa quotes with Sree gloss, closing pull-quote, guest card. YouTube: https://youtu.be/a8ap2LJTSNk. `/conversations/roopa-sreeranganna.html`
- **The builder who bounces back — Tuhin Mohanta** — second episode. Sree with Tuhin (20 years of building, a Bengal childhood that taught him to find rhythm inside chaos, an inflection point read as a reset). 52 minutes. Themes: structure hidden inside chaos, the cork that won't stay down, building as identity. YouTube ID `IbhqHXLJYuY`. `/conversations/tuhin-mohanta.html`
- **Three decades, five machines — Sivarama Sundar** — third episode, **first audio-only one** (a video take was discarded — Siva is at his best off camera; re-recorded as a voice call while Sree walked 8 km). 1 hr 41 min, June 2026. The journey: Pollachi → a library childhood → Prince of Persia ('92) → NIIT at sixteen → the raindrops virus in assembly → ₹750 first paycheck for a flour-mill app → Deccan Herald classified + a four-hour first interview (June '95) → Clipper for factories ("we even collected the cheques") → IICODE/Everest and the Delphi decade → German ASP, first team of 20 → Euro Brokers Wall Street milliseconds → Mercantila ($70M, store in 48 hrs; mentor Bala, TPS/lean) → Philips cath-lab platform → Tesco Clubcard re-architecture (the no-code socket system that ran decades without downtime) → today: a 12-week future-engineers practice inside a consulting firm + AI platforms. AI themes: the point of no return ("you can't unsee it"), articulation as the new skill, tokens as the new-age currency, advice to four generations, AI's side effect of making us better humans, the "bitter pill" (plastics / coal-per-megabyte analogies), India and IP. Closing line: "Happy to leave any tiny breadcrumbs that we could, to bring in change." `/conversations/sivarama-sundar.html`. **Pending: real YouTube ID** (placeholder `YOUTUBE_VIDEO_ID_HERE` in the page's bottom script).

### Sparks live
- **Should I walk or drive?** — the circle's first spark. Venkata Rajesh Solasa shared a screenshot of an AI confidently telling someone to *walk* to a car wash 100m away; the group chat turned it into a thread on clear prompting (Abhiram J), clear communication as a leadership trait (Vikas Anand), context-awareness (Tuhin Mohanta), the Mahābhārata's Aśvatthāmā half-truth (Vikas — *"Context is everything"*), and a grounded resolution (Vaskar Nag — *"good to walk to collect your car"*). The exchange is rebuilt on the page as **chat bubbles, not screenshots** (a dark CSS Claude card + a WhatsApp-style thread), with Sree's framing prose and a `.gloss` aside on the Aśvatthāmā story. Curated by Sree Balakrishnan. `/sparks/context-is-everything.html`

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
