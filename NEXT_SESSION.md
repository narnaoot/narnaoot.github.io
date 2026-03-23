# Next Session Handoff

## What's done

- `Inspiration.md` fully documented with file references, 5 designers + Stephen's Game of Life analyzed
- Site pages exist: index, about, work, method, fave (alternate hero)
- Branch: `claude/rebuild-index-page-b1pLZ`

## What was planned but NOT built yet

Everything below goes in a **new `redesign/` folder** — do NOT overwrite existing files.

---

### 1. `redesign/about.html`

Start from `about.html` and add these new sections (in this order):

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

**D. Enhanced Testimonials (add to existing)**

Use he/him pronouns and name Nabil throughout (LinkedIn recs use old name Nadya + she/her — adapt them).

New ones to add (in addition to 6 already on the page):
- **Brianna Gamp** (Info Security Leader): "He has the unique ability to walk into an ambiguous situation, quickly grasp the key milestones and action items, identify technical needs that have not been addressed, and get results — all while getting a smile out of everyone in the room."
- **Salathiel Bluitt** (Accenture): "He is a hard-working self-starter who invariably understands exactly what a project is all about from the outset, and how to get it done quickly and effectively... I cannot remember an instance in which he missed a major deadline."
- **Teja** (colleague): "I'm the reason she joined our team — I was her first interview. She really liked our conversation and that I was honest."  ← keep this verbatim, it's a she/her speaker describing her own experience
- **Cliff Winnig**: "Resilience, empathy, and consistently logical thinking."
- **Debbie** (friend): Three-part: (1) extraordinarily good at nuanced and complex self-care; (2) self-care skills are why he's so good at caring for others; (3) true lifelong learner — never known him when he wasn't trying to learn or expand a skill.
- **Tom** (family friend, via Nabil's mom): "You could feel the compassion and love he has for people."
- **Laura** (friend): "My smarts and my bounce — like Tigger."

Skip (too personal/intimate for site): Heidi's quotes, Sarat's quotes, the "totally hot" quote, Linae's quote, Tekla's romantic quote.

**E. Things I Love — Icon Grid**
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

### 3. `redesign/career-river.html` (or a section within about) — Animal Crossing River

Inspired by **Stephen's Game of Life** (`inspiration_samples/Stephen's Game of Life.png`):
- Stephen used an actual Game of Life board — winding path, company logos as stops, callout boxes in margins
- **Nabil's version:** same concept but as an **Animal Crossing–style river** — Nabil is floating on a tube, drifting downstream past career stops
- Each stop = a job/era (landmark on the riverbank: Apple = apple tree, SFMTA = cable car stop, Saint Mary's = a little school, etc.)
- Callout boxes floating near each stop with dates + one-sentence description
- Tone: warm, playful, slightly whimsical — matches the "nerd and fairy" energy
- This could be a static SVG illustration OR a simple CSS/HTML layout with a wavy river shape

**Still needs from Nabil:** approval of the concept and any specific landmarks/details he wants per stop

---

## Nabil's questions for you (things that need his input to finish)

1. **Career excitement chart** (Catherine Madden #1 style, `Resume+-+13.webp`) — needs excitement levels for each role:
   - Elegrity (2006–2010)
   - eBay (2010–2011)
   - Apple Eng PM (2011–2014)
   - Apple Process Eng (2014–2020)
   - St. Mary's / consulting (2020–2024)
   - SFMTA (2024–now)

2. **Books I've read** — for a Catherine Madden #7 style bubble chart (inspo `Resume+-+14.webp`): what books should be on it?

3. **The "Mary" attribution** — does he want to name her, or keep it as "A friend"?

4. **Teja quote** — she/her speaker, quote references Nabil but uses third person. Fine to include as-is?

---

## Technical notes

- All new files go in `redesign/` folder only
- Keep existing files completely untouched
- Same CSS tokens and fonts as existing pages
- Push to `claude/rebuild-index-page-b1pLZ`
