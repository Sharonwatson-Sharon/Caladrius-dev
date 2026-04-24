# Caladrius Health.AI — Claude Context

## Project Overview
Jekyll-based website for Caladrius Health.AI, a technology company developing NHCX-aligned solutions for healthcare providers in India.

- **Live site:** https://sharonwatson-sharon.github.io/Caladrius-dev/
- **Repository:** https://github.com/Sharonwatson-Sharon/Caladrius-dev.git
- **Branch:** `main` (auto-deploys to GitHub Pages on every push)

---

## Stack
- **Framework:** Jekyll 4.4.1
- **Ruby:** 3.3.11
- **Theme:** Minima (default Jekyll theme)
- **Hosting:** GitHub Pages via GitHub Actions

---

## Project Structure

```
├── _posts/                    # Blog articles (YYYY-MM-DD-title.markdown)
├── _config.yml                # Jekyll site configuration
├── .github/workflows/
│   └── jekyll.yml             # GitHub Actions build & deploy workflow
├── index.markdown             # Homepage — links to both homepage versions + blog
├── blog.markdown              # Blog listing page (/blog/)
├── about.markdown             # About page
├── caladrius-homepage.html    # Homepage Version 1 (V3 standalone bundled file)
├── caladrius-homepage-v2.html # Homepage Version 2 (caladrius-homepage-final)
├── Gemfile                    # Ruby gem dependencies
└── Gemfile.lock               # Locked gem versions (includes x86_64-linux for CI)
```

---

## Work Log

### 2026-04-24 — Initial Setup
- Installed Ruby 3.3.11 (via winget) and Jekyll 4.4.1 + Bundler
- Scaffolded Jekyll site in `C:\Users\Lenovo\Caladrius-dev`
- Added Homepage Version 1 (`caladrius-homepage.html`) — V3 standalone bundled file
- Added Homepage Version 2 (`caladrius-homepage-v2.html`) — caladrius-homepage-final
- Built custom homepage (`index.markdown`) with links to both versions and blog
- Added blog post: *"Beyond NHCX: Global Claims Exchange Models and What They Mean for India"* (`_posts/2026-04-07-beyond-nhcx-global-claims-exchange-models.markdown`)
- Created `/blog/` listing page (`blog.markdown`)
- Configured GitHub Actions workflow for automated Jekyll deployment
- Fixed `Gemfile.lock` to include `x86_64-linux` platform for Ubuntu CI runner
- Site successfully deployed to GitHub Pages

---

## Deployment
Every push to `main` triggers the GitHub Actions workflow at `.github/workflows/jekyll.yml`, which builds the Jekyll site and deploys it to GitHub Pages automatically.

To run locally:
```bash
bundle exec jekyll serve
```
Visit `http://localhost:4000`.

---

## Notes
- Homepage versions are served as static HTML files (no Jekyll front matter) — Jekyll passes them through as-is
- Blog posts go in `_posts/` with filename format `YYYY-MM-DD-title.markdown` and require Jekyll front matter
- The `Gemfile.lock` must include `x86_64-linux` platform — run `bundle lock --add-platform x86_64-linux` if adding new gems on Windows
