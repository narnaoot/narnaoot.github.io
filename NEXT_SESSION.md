# Next Session Handoff

## What's done

- `Inspiration.md` fully documented with file references, 5 designers + Stephen's Game of Life analyzed
- Root site pages updated: index, about, work, method — all reframed from "data storyteller" to **Project Leader**
- Branch: `claude/redesign-personal-website-oIzoy`

### Root page changes made (session 2)

- **index.html**: title/tagline → "Project Leader"; about lead/body copy reframed around PM clarity
- **about.html**: section headers updated; English Lit note reframed; 9 new PM-focused testimonials added (Wanda Davis, Faron Lyons, Karina Sanz, Salathiel Bluitt, Brianna Gamp, Cliff Winnig, Séain Gutridge, Tom, Laura)
- **work.html**: iTunes project reframed as PM story (tags: Project Management / Process Design / Cross-functional / Automation); SHAP project reframed toward stakeholder translation; career chain caption updated
- **method.html**: skill columns reordered — "Project & Program Leadership" leads; "Data & Analysis" → "Analysis & Insight"; "Data Storytelling" → "Translating Complexity"

---

## All inspiration files (quick reference)

Full notes on each are in `Inspiration.md`. Every file is in `inspiration_samples/`.

| File | Designer | What it is |
|------|----------|------------|
| `Resume+-+13.webp` | Catherine Madden | Career excitement bubble chart — X=time, Y=excitement, bubbles=skills/focus areas |
| `Resume+-+12.webp` | Catherine Madden | Bell curve — X=creative freedom, Y=job satisfaction; peak = trust/vision/leadership |
| `Resume+-+11.webp` | Catherine Madden | 2×2 quadrant on dark bg — business vs pleasure × solo vs group; shows change over time |
| `Resume+-+8.webp` | Catherine Madden | Life stages stacked bar / stream chart — age 0–30, color bands = how time was spent |
| `Resume+-+14.webp` | Catherine Madden | "My Favorite Tools" — stacked bar by age showing how creative tools evolved |
| `Emy1.webp` | Catherine Madden | Radial/donut "Inspiration" chart — self-portrait at center, segments = sources |
| `Emy3.webp` | Catherine Madden | "Books I've Heard Lately" bubble chart — X=fact/fiction, Y=bored/obsessed |
| `Nina1.webp` | Unknown (Tableau blog) | Dual-track horizontal timeline — career below the line, creative output above |
| `image4_0.png` | Nina Voordes | Full portrait infographic — dot matrix skills, hex tools, "Things I ♥" icon grid at bottom |
| `Stephen's Game of Life.png` | Stephen (Tableau blog) | Career as a Game of Life board — winding path, company logos as stops, callout boxes |
| `JRashVisualResume___.jpg` | Jennifer Rash | 3×3 grid of color-coded circles on black — color = era, diagonal connectors = transitions |
| `CV  Resume.png` | Samuel Parsons | Dark charcoal, landscape — radial arc timeline + "Core Values" text + bubble cluster of work |
| `website/inspo1.pdf` | Stefanie Kraus | Portfolio homepage — project cards, long-form testimonials, single CTA |
| `website/inspo2.pdf` | Stefanie Kraus | "My Process" page — 7 numbered steps with AI woven in naturally |
| `website/inspo3.pdf` | Stefanie Kraus | Full about page — career origin story, FAQ format, personal interests at bottom |

---

## What needs building in `redesign/`

All new files go in a **`redesign/` folder** — do NOT overwrite existing root files.

---

### 1. `redesign/about.html`

Start from updated `about.html` and add these new sections (in this order):

**A. Bell Curve — "My Professional Sweet Spot"**
- Inline SVG, inspired by Catherine Madden inspo `Resume+-+12.webp`
- X-axis: "Rigid Process" → "Pure Chaos"
- Y-axis: "Energy & Joy"
- Peak label: "TRUST · TRANSLATION · 0→1"
- Left tail note: "Just executing, not thinking"
- Right tail note: "No constraints, nothing lands"
- Colors: teal fill (semi-transparent), coral stroke

**B. Three Pillars — Mary's Analysis**
- Three-column card layout
- Source: a friend named Mary wrote a character analysis with three named categories:
  1. **Networked Intelligence** — "The way you stay involved in what's happening in the world... bring super smart analysis... go deep very quickly... make connections across a wide range of topics... your mind involving a lot of heart, and being very fast."
  2. **Fierce Advocacy** — "You stand up for people you care about... you seem to know what you can't compromise... generous with the people and animals around you."
  3. **Incorruptible Practicality** — "Moving forward in a world that doesn't have you in mind... extremely honest... accounts for the fact that some structures will take time to dismantle... you find your way to be true to yourself and also pick your battles."
- Attribution uncertain ("I think this was Mary?") — attribute as "A friend"

**C. Teaching Vignette Card**
- Narrative card telling this story (not a blockquote — a 3–4 sentence story):
  - Week before midterms: 3 of 6 MS cohort classmates asked for help with SQL
  - He held a 1–2 hour session walking through how SQL works
  - Mark and Nupur both said it made a decisive difference on the midterm
  - Nupur asked to use 4 hours of class time to go over material with him instead of class
  - Ipsita's full text: "Nabil - I can only say Thank you for everything. But you deserve more. I've learned a lot of things from you. I really appreciate the way you explain, the way you solve a problem, the way you help us and the way you talk."
  - Separately: Nupur said she wants to learn from him how to speak up in the moment — she described a moment in office hours where Nabil calmly but firmly told a dismissive professor "When I ask a question I've already tried to figure it out, I would really like an answer."

**D. Things I Love — Icon Grid**
- Inspired by Nina Voordes (image4_0.png bottom section)
- Simple emoji + label grid, ~4 columns:
  - 🐱 Octavia & Cleopatra
  - 🍵 Tea (always)
  - 📚 All the books
  - 🏙️ San Francisco
  - 🚌 City transit
  - 📊 Data stories
  - ∞ 0→1 problems
  - 🤝 Teaching & mentoring
  - 🌿 Secret gardens
  - 🎲 Statistics & probability
  - 🖊️ English Lit (UChicago, always)
  - 🤖 Making ML human

---

### 2. `redesign/index.html`

Cleaner homepage inspired by Stefanie Kraus (inspo1–3 PDFs):
- Simpler hero (shorter, warmer)
- Chris Winter robot quote as a large featured pull quote near the top
- Projects section (same 3 cards as existing)
- Single CTA footer

---

### 3. `redesign/career-river.html` — Animal Crossing River

Inspired by **Stephen's Game of Life** (`inspiration_samples/Stephen's Game of Life.png`):
- Same concept but as an **Animal Crossing–style river** — Nabil floating on a tube, drifting downstream past career stops
- Each stop = a job/era (landmark on the riverbank: Apple = apple tree, SFMTA = cable car stop, Saint Mary's = a little school, etc.)
- Callout boxes floating near each stop with dates + one-sentence description
- Tone: warm, playful, slightly whimsical
- Static SVG illustration OR simple CSS/HTML layout with a wavy river shape

**Career stops:**
- Elegrity (2006–2010) · Engineering PM
- eBay (2010–2011) · Program Manager
- Apple (2011–2014) · Engineering PM · project-level
- Apple (2014–2020) · Process Engineer · org-wide
- St. Mary's / consulting (2020–2024)
- SFMTA (2024–now) · Principal Business Analyst

---

## Nabil's open questions

1. **Career excitement chart** (Catherine Madden #1 style) — needs excitement levels per role to build the chart
2. **Books** — for a bubble chart: which books to include?
3. **Mary attribution** — name her, or keep as "A friend"?
4. **Teja quote** — she/her speaker, third person about Nabil. Fine to include as-is?

---

## Technical notes

- All new files go in `redesign/` folder only
- Keep existing root files untouched
- Same CSS tokens and fonts as existing pages
- Push to `claude/redesign-personal-website-oIzoy`
