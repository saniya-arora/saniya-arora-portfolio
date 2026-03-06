# Saniya Arora — Code + Canvas + AI

Personal portfolio site for Saniya Arora, a product designer building enterprise platform systems at the intersection of code, canvas, and AI.

**Live sections:** Hero, How I Work, Impact, Selected Work, Side Quests, About, Footer/Contact

## Overview

A single-page portfolio built with vanilla HTML, CSS, and JavaScript — no frameworks, no build step. The design follows a dark-first, editor-inspired aesthetic with a dot-grid canvas background, monospace accents (JetBrains Mono), and a cohesive green accent color system.

## Structure

| Section | What it covers |
|---|---|
| **Hero** | Tagline, intro copy, and an interactive LLM-style chat window that greets visitors and tailors responses based on who they are (recruiter, hiring manager, designer, engineer, or just browsing). |
| **How I Work** | A three-column animated pipeline — Canvas → Specs → Agents — showing how design problems move from brief to structured spec to AI agent execution. Includes staggered reveal animations and a cycling agent-status simulation. |
| **Impact** | Four metric cards summarizing outcomes: platforms shipped, design cycle speed gains, 0→1 product launches, and cross-org alignment. |
| **Selected Work** | Case study cards styled as editor panels, linking out to dedicated pages for Locksmith (identity platform), WAVE (AI orchestration framework), John Deere (digital twin UX), and Airkey (cross-channel verification). |
| **Side Quests** | Three personal projects — Between (letter-sharing app), this portfolio itself, and FinanceHQ (financial prompt builder). |
| **About** | Background and thought leadership topics. |
| **Footer** | Contact links (email, resume PDF, LinkedIn) and copyright. |

## Key Features

- **Dark / Light theme toggle** — persists choice to `localStorage`, respects `prefers-color-scheme` on first visit, and updates the `<meta name="theme-color">` for mobile browsers.
- **Interactive chat widget** — a simulated LLM conversation in the hero section. Visitors pick a role chip; the agent types out a tailored response with a blinking cursor, then reveals a contextual CTA.
- **Scroll-triggered reveals** — lightweight `IntersectionObserver`-based fade-in animations on every major section, with `prefers-reduced-motion` support that disables all transitions.
- **How I Work agent animation** — panels stagger in on scroll; agent rows slide in sequentially then cycle through thinking → done states on a loop.
- **Fully responsive** — three breakpoints (920px, 860px, 640px) collapse grids and hide the nav link bar on mobile.
- **Zero dependencies** — no npm, no bundler, no external JS. Fonts are loaded from Google Fonts; everything else is self-contained.

## Tech

- **HTML5** — semantic markup, ARIA labels on decorative elements and landmarks.
- **CSS** — custom properties for theming, `clamp()` for fluid typography/spacing, `color-mix()` for the translucent nav, CSS Grid and Flexbox layouts.
- **JavaScript** — vanilla ES5-compatible; handles theme persistence, scroll reveals, chat interaction, and the agent cycle animation.
- **Fonts** — Inter (sans-serif) and JetBrains Mono (monospace) via Google Fonts.

## Case Study Pages

Each work card links to a dedicated HTML page in the same directory:

| File | Project |
|---|---|
| `locksmith.html` | Locksmith — AI-driven self-service identity platform |
| `wave.html` | WAVE — Multi-agent AI orchestration framework |
| `johndeere.html` | John Deere — Digital twin for equipment operators |
| `airkey.html` | Airkey — Cross-channel verification redesign |

## Running Locally

No build step required. Open `index.html` in any modern browser, or serve the directory with any static server:

```bash
# Python
python3 -m http.server 8000

# Node (npx)
npx serve .
```

## Contact

- **Email:** saniyaaroraux@gmail.com
- **LinkedIn:** [linkedin.com/in/saniya-arora-20](https://www.linkedin.com/in/saniya-arora-20)
