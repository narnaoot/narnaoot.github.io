# narnaoot.github.io — Nabil Arnaoot's Personal Site
# Check the folders to see earlier versions of the website Claude designed for me.

A personal portfolio site for Nabil Arnaoot: Principal Business Analyst, Project Leader, translator of complexity. Currently working at SFMTA.

## Emphasis

The site foregrounds **project leadership** — Nabil's ability to walk into ambiguous situations, define problems, build cross-functional processes, and deliver results. Data skills are a supporting capability, not the headline.

## Site structure

### Root (live site — do not touch)

| File | Purpose |
|------|---------|
| `index.html` | Homepage |
| `about.html` | Personal portrait, testimonials, education |
| `work.html` | Project case studies |
| `method.html` | How Nabil works |

### redesign/ (active development)

| File | Purpose |
|------|---------|
| `redesign/index.html` | Homepage |
| `redesign/work.html` | CareerRiver image, 4 case studies |
| `redesign/method.html` | 6 diagnostic questions, Duct Tape/Drano, animated skill bars |
| `redesign/about.html` | 4 sections: personal portrait, three pillars, teaching vignette, things I love |
| `redesign/testimonials.html` | "Praise" page — 15 testimonials + education & certifications |

## Design tokens (in every page's `:root`)

| Token | Value | Use |
|-------|-------|-----|
| `--coral` | `#E8614F` | Primary accent, nav logo |
| `--teal` | `#2DB5A8` | Secondary accent |
| `--mustard` | `#D4920A` | Tertiary |
| `--lavender` | `#8B7BC8` | About/Praise hero kicker + accents |
| `--sage` | `#6A9F7A` | Soft accent |
| `--bg` | `#FFFBF5` | Page background (warm cream) |
| `--text` | `#3D2B1F` | Body text (dark brown) |

Fonts: **Playfair Display** (headings) + **Nunito** (body)

## Images

Section thumbnails live in `redesign/` (same folder as HTML). Referenced with simple relative paths (e.g. `src="AboutHero.png"`).

| File | Use |
|------|-----|
| `redesign/AboutHero.png` | about.html — "The Human Behind the Projects" |
| `redesign/ThreePillars.png` | about.html — "Three Things I Always Bring" |
| `redesign/ThingsILove.png` | about.html — "Things I Love" |
| `redesign/Testimonials.png` | testimonials.html — "What People Say" |
| `redesign/Education.png` | testimonials.html — "Education & Certifications" |
| `redesign/TeachingScene.png` | about.html — "One More Thing" |
| `redesign/ProfilePicture.jpeg` | about.html hero avatar |
| `inspiration_samples/CareerRiver.png` | work.html career river illustration |

## Inspiration research

See `Inspiration.md` for full notes. Key reference designers:
- **Catherine Madden** — data viz as personality expression
- **Stefanie Kraus** — clean, warm, testimonial-forward portfolio
- **Nina Voordes** — dual-track timeline, icon grids
- **Jennifer Rash** — bold, project-first
