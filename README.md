# narnaoot.github.io — Nabil Arnaoot's personal site

Personal portfolio for Nabil Arnaoot — Principal Business Analyst and project leader at SFMTA. Plain static HTML, deployed via GitHub Pages at **n4bil.com** (see `CNAME`).

## Emphasis

Foregrounds **project leadership** — walking into ambiguous situations, finding the real problem, building the process that's missing, and delivering. Data/analytics is a supporting capability, not the headline.

## Site structure (all live, at repo root)

| Page | Contents |
|------|----------|
| `index.html` | Home — hero (portrait, "0 → 1 is infinite", intro) · KPI panel (3 dashboard-style tiles, each clicking through: 25+ years with a sector split bar → `work.html#career`; 500K systems → `work.html#kernel`; Tiptree nomination → `about.html#writing`) · pull quote · "The work, briefly" + career/education line · selected-work teaser + Patterns/About cards |
| `work.html` | 3 deep case studies (eBay, iTunes, Kernel) · What People Say (testimonials) · Career: river illustration + one-line dated career history (`#career`) · 4 side quests linking to the note pages |
| `patterns.html` | Favorite questions · Two Kinds of Problems (Duct Tape / Drano) · Everything Starts on a Whiteboard · Microchipping Sheep |
| `about.html` | Short personal intro (English Lit, SF, feral cats) · Three Things I Always Bring (Mary Salome) · Teaching and Writing (`#writing`) · education |
| `gardens.html` | Secret Gardens of San Francisco — Tableau embed |
| `probability.html` | Conditional Probability for Normal Humans — essay + tables |
| `unicorns.html` | Chasing Unicorns for Pride — Tableau embed |
| `nametag.html` | Nametag — landing page for a prototype web app: app screenshot, "Try it" link-out, and a mailto feedback form |

Masthead nav (4 main pages): Home · Work · Patterns · About. The four note/side-quest pages link back from Work.

## Design system

Shared styles live in **`css/styles.css`**: the `:root` tokens, reset, masthead/nav, section headings, the stacked page header used by Work/Patterns/About (`.page-hero`), the note-page hero + back link, Tableau embed styles, the footer (including the Cleo and "Built by" credit lines), and a `scroll-margin-top` so `#anchor` links clear the sticky masthead. Each page sets its accent with two variables in a small inline `<style>` (`--accent` for fills/underlines, `--accent-ink` for accent text) and keeps only its page-unique styles inline.

Each page's signature accent colors the wordmark, nav underline, and footer/button chrome:

| Page | Accent |
|------|--------|
| Home | orchid |
| Work | coral |
| Patterns · Unicorns | teal |
| About | lavender |
| Gardens | sage |
| Probability | mustard |
| Nametag | blush |

Shared palette: warm cream `--bg #FFFBF5`, ink `--text #3D2B1F`, `--muted #7C6151`; accents `--coral #F5563F`, `--teal #12C2B0`, `--mustard #F0A500`, `--sage #4FB870`, `--lavender #9B6DE8`, `--orchid #A75FA0` (plus `--denim`, `--blush`, `--citron`). Each accent has a deep `-dk` cut for legible colored text on tinted backgrounds (e.g. `--teal-dk #14655D`), so text-on-tint pairings clear WCAG AA.

Fonts: **Libre Caslon Text** (serif headings) + **Nunito** (body).

### Design guardrails (from the Sep 2026 AI-cliché passes)

The site was deliberately stripped of template/AI-generated tells. Keep it that way:

- **No pill tags** after section headings, and no rows of keyword/skill chips.
- **Accent-colored heading word only on the Home hero** ("infinite"); other headings stay one color.
- **No spaced-out ALL-CAPS labels** (the masthead nav is the one exception). Small labels are plain text in the accent ink.
- **No gradients, giant decorative quote marks, or decorative drop shadows.** Tinted boxes are flat single colors, used sparingly.
- **No grids of identical pastel cards or ghost "01/02/03" numerals**; prefer plain prose or text columns with a thin accent rule.
- **KPIs are dashboard-style**: value in text color, label above, context below, and a click-through to the detail (landing on the right section, not the top of a page).
- **Page tops use the shared stacked `.page-hero`** (title, then intro beneath), not a title-left / intro-right split.
- **Kept on purpose:** the painted Before/After case-study illustrations, the Duct Tape / Drano art, and the cowboys / microchipping-sheep metaphor on Patterns.

## Assets

Assets live under `assets/` (the HTML pages, `CNAME`, and `README.md` stay at root). All illustrations are WebP (converted from source PNG/JPEG; the originals remain in git history).

- **`assets/img/`** — 14 `.webp` images + `Monogram.svg`:

  | File | Where used |
  |------|------------|
  | `Monogram.svg` | masthead logo (all pages) |
  | `ProfilePicture.webp` | Home hero portrait + About header avatar |
  | `CleoInspects.webp` | "Inspected by Cleo" footer (all pages) |
  | `CareerJourneyPainted.webp` | Work — Career section (the river illustration is the career timeline; two painted signpost dates are out of date, see `plan/NEXT_SESSION.md`) |
  | `LighthousePainted.webp` | Work — eBay case study |
  | `QuietedPagersPainted.webp` | Work — iTunes case study; also the Home teaser thumbnail |
  | `KernelCleanupPainted.webp` | Work — Kernel case study |
  | `ThreePillarsPainted.webp`, `TeachingScene.webp`, `EducationWalkPainted.webp` | About section thumbnails (Three Things, Teaching and Writing, Education) |
  | `WordCloudsPainted.webp` | Work — What People Say thumbnail |
  | `duct_tape.webp`, `drano.webp` | Patterns — Two Kinds of Problems panels |
  | `microchip.webp` | Patterns — Microchipping Sheep (whiteboard photo) |
  | `Nametag.webp` | Nametag — app home-screen screenshot (resized + converted from the uploaded `Nametag.png`, which remains in git history) |

- **Removed Sep 30:** `assets/icons/` (the Home hero chips and About portrait cards that used them are gone; recover with `git checkout ba0be56 -- assets/icons`) and `assets/img/AboutHero.webp` (thumbnail for the old About portrait cards; recover with `git checkout abb3aeb -- assets/img/AboutHero.webp`).

The repo now holds only what the live site uses. Prior source PNG/JPEG originals, reference imagery (`inspiration_samples/`), and old site versions were removed from the working tree and remain in git history.

## Working notes

- `plan/NEXT_SESSION.md` — running handoff / review log and current open items.
- `plan/Inspiration.md` — design research and reference designers (its image links point at the removed `inspiration_samples/`; the notes still read fine, images are in git history).
