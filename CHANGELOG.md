# Changelog

All notable changes to the Caladrius Health.AI website are recorded here in reverse chronological order.

---

## [2026-04-24]

### Added
- `CLAUDE.md` — project context and work log for Claude Code sessions
- `README.md` — project setup summary, local dev instructions, and file structure
- `blog.markdown` — blog listing page at `/blog/`
- Blog post: *"Beyond NHCX: Global Claims Exchange Models and What They Mean for India"* (`_posts/2026-04-07-beyond-nhcx-global-claims-exchange-models.markdown`)
- `caladrius-homepage-v2.html` — Homepage Version 2 (caladrius-homepage-final)
- `caladrius-homepage.html` — Homepage Version 1 (V3 standalone bundled file)
- `.github/workflows/jekyll.yml` — GitHub Actions workflow for automated Jekyll build and deployment to GitHub Pages
- Initial Jekyll site scaffold (`_config.yml`, `Gemfile`, `index.markdown`, `about.markdown`, `404.html`, `_posts/`)

### Changed
- `index.markdown` — replaced default home layout with custom page linking to both homepage versions and the blog
- `Gemfile.lock` — added `x86_64-linux` platform to support GitHub Actions Ubuntu runner

### Infrastructure
- Installed Ruby 3.3.11 (via winget) and Jekyll 4.4.1 + Bundler 4.0.10
- Connected local repo to `https://github.com/Sharonwatson-Sharon/Caladrius-dev.git`
- Enabled GitHub Pages — site live at `https://sharonwatson-sharon.github.io/Caladrius-dev/`
