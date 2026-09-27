# Engineering Portfolio Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Convert the Academic Pages template into Hyuneun Seo's factual, project-first engineering portfolio.

**Architecture:** Keep Jekyll and Academic Pages collections. Put verified identity and links in `_config.yml`, structured experience and publications in `_data/cv.json` and collection files, and use a focused home/project presentation with small SCSS additions rather than a frontend rewrite.

**Tech Stack:** Jekyll, Liquid, Markdown, YAML, JSON, SCSS, GitHub Pages.

**Spec:** `docs/superpowers/specs/2026-09-28-engineering-portfolio-design.md`

## Global Constraints

- Keep Academic Pages/Jekyll and its existing collection model.
- Use a restrained light theme with dark text, one technical accent color, compact cards, and strong whitespace.
- Make projects the first substantial content after the hero.
- Preserve static-site performance: no new frontend framework, no heavy runtime dependencies, and no unnecessary external assets.
- Do not invent dates, metrics, employers, repository URLs, paper titles, venues, or awards.
- Do not imply real-robot operation, real-flight deployment, or closed-loop robot control.

## Review Focus

- Placeholder identity or sample content remains visible — search rendered output and source collections for template text.
- A project claim exceeds the verified evidence — inspect each project copy against the existing context and source files.
- A missing image or external asset breaks the page — build with network-independent local assets where possible.
- Mobile project cards overflow — inspect responsive CSS and rendered narrow layout.
- GitHub Pages/Jekyll build fails — run the repository's supported build command before completion.

### Task 1: Replace site identity and navigation

**Files:**
- Modify: `_config.yml`
- Modify: `_data/navigation.yml`
- Modify: `_includes/sidebar.html` only if the existing author fields cannot express the verified profile

- [ ] Update site title, description, author name, bio, location, GitHub, and other links using only verified values.
- [ ] Configure navigation for Home, Projects, Publications, CV, and About; remove sample sections from the menu.
- [ ] Search configuration and navigation for remaining template identity values.
- [ ] Run the Jekyll build and confirm configuration parses.

### Task 2: Build the project-first home page

**Files:**
- Modify: `_pages/about.md`
- Create: `_pages/projects.md`
- Modify: `_sass/layout/_page.scss` or create a focused portfolio partial under `_sass/`

- [ ] Replace the Academic Pages instructional home content with an engineering positioning hero and verified capability summary.
- [ ] Add a project grid or compact project list driven by the portfolio collection, with links to detail pages.
- [ ] Add a short research snapshot covering ongoing multimodal/facial-coordination work without clinical claims.
- [ ] Add clear CV, GitHub, and contact actions only when URLs are verified.
- [ ] Add responsive styles for the hero and cards, then build and inspect the home page output.

### Task 3: Add verified engineering project content

**Files:**
- Delete or replace: `_portfolio/portfolio-1.md`, `_portfolio/portfolio-2.html`
- Create: `_portfolio/etri-gnss-denied-localization.md`
- Create: `_portfolio/edge-deployment.md`
- Create: `_portfolio/safe-landing.md`
- Create: `_portfolio/validation-tooling.md`
- Create: `_portfolio/backend-cloud-cicd.md`

- [ ] Use clean filenames and front matter compatible with the existing `portfolio` collection.
- [ ] Write concise project summaries describing problem, engineering contribution, stack, and evidence.
- [ ] Mark simulation/research/deployment boundaries explicitly where relevant.
- [ ] Reuse a local project image only when it genuinely explains the project; otherwise use a text-first card.
- [ ] Build and verify every project permalink resolves.

### Task 4: Replace CV and publication placeholders

**Files:**
- Modify: `_pages/cv.md`
- Modify: `_data/cv.json`
- Replace: `_publications/*.md` with verified entries only
- Modify: `_pages/cv-json.md` if the JSON CV remains in navigation

- [ ] Replace sample education, work, skills, and publication data with verified facts.
- [ ] Preserve real publication title, venue, author, date, PDF, and award information only when available in the project context or repository.
- [ ] Remove fake sample talks, teaching, and placeholder papers.
- [ ] Build and inspect CV and publication pages for missing fields and broken links.

### Task 5: Clean template residue and verify presentation

**Files:**
- Modify or remove only confirmed sample pages under `_pages/`, `_posts/`, `_talks/`, and `_teaching/`
- Modify: `_config.yml` or collection settings if needed to hide unused collections

- [ ] Remove sample content from navigation and generated output without touching Academic Pages framework files unnecessarily.
- [ ] Search source and generated output for `Your Name`, `GitHub University`, `Paper Title Number`, and other sample strings.
- [ ] Run the full local build and check for warnings/errors.
- [ ] Preview home, projects, publications, and CV pages at desktop and narrow widths.
- [ ] Review `git diff` for factual overclaiming, accidental template deletion, and unrelated changes.
