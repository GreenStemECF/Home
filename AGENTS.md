# AGENTS.md

## Purpose
This repository is a static website for the Green Stem Educational and Charitable Foundation. The site is composed of root-level HTML pages, static CSS/JS assets, and a GitHub Pages deployment workflow.

## What an AI agent should know
- This is a static content site, not a web app with a backend.
- The main pages are in the repository root: `index.html`, `CallForAbstract.html`, `OurJourney.html`, `Symposium2024.html`.
- Styling is served from `css/`; there is also source Sass in `scss/`.
- JavaScript lives in `js/`; assets live in `images/` and `fonts/`.
- There is no `package.json`, `npm`, `yarn`, or other package manager metadata present.
- The repository deploys directly to GitHub Pages using `.github/workflows/static.yml`.

## Editing guidance
- Prefer editing the rendered HTML and static CSS when making site changes.
- If changing styles, keep `css/` and the Sass sources in `scss/` consistent.
- Do not introduce build tooling assumptions unless the user explicitly adds a build configuration.
- Keep changes compatible with GitHub Pages deployment from the repository root.

## Deployment
- Pushes to `main` trigger `.github/workflows/static.yml` to deploy the repository content to GitHub Pages.

## Key files and directories
- `index.html` — homepage
- `CallForAbstract.html`, `OurJourney.html`, `Symposium2024.html` — secondary pages
- `css/` — deployed stylesheets
- `scss/` — Sass source files, including Bootstrap sources
- `js/` — client-side script files
- `images/` and `fonts/` — static assets
- `.github/workflows/static.yml` — GitHub Pages deploy pipeline
