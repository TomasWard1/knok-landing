# Knok Landing

## Stack
- **Framework:** Astro
- **CSS:** Tailwind v4 (inline classes, CSS vars for design tokens)
- **Deployment:** Vercel

## Branch Strategy
- `main` = production
- `staging` = integration branch (all PRs target here)
- `feat/*`, `fix/*`, `chore/*` = development branches (from staging)

## Design
- Design file: `design/knok-landing.pen` (Pencil — not tracked in git)
- Design system: brutalist, black/white + red accent (`#FF2400`)
- Font: Inter
- CSS variables defined in `src/styles/global.css`

## i18n
- Inline in `src/pages/index.astro` — `en` and `es` objects at the top
- Toggle via `#lang-toggle` button, handled in inline `<script>`

## Key Files
- `src/pages/index.astro` — entire page (single-file)
- `src/layouts/Layout.astro` — HTML shell
- `src/styles/` — global CSS with Tailwind v4 theme vars

## Notes
- Star count fetched client-side from GitHub API
- Release URL / repo URL defined as constants near top of `index.astro`
