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
/                        → index.html                 Homepage (CLC hub — who we are, how we gather, founding members)
/the-same-question       → the-same-question.html     Article: Luddite comic, gate, founding story, Sunil's pillars
/lotus                   → lotus.html                 Article: Buddhism, Taoism, Stoicism, Gita — four traditions
/puzzle                  → puzzle.html                Dormant redirect to / — do not edit for content
/origins                 → origins.html               Dormant — superseded by the-same-question.html
```

> **Important:** Edit `index.html` directly for homepage changes. `puzzle.html` and `origins.html` are dormant legacy files.

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

### Articles teased / in progress
- **The Same Question** — the Luddite comic and founding story (origins.html)
- **The Ancient Answer** — Gita / Buddhism / Stoicism philosophical piece (the-lotus.html)

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
