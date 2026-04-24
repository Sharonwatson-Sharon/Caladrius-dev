# Caladrius Health.AI — Website

Live site: **https://sharonwatson-sharon.github.io/Caladrius-dev/**

---

## Setup Summary

### 1. Environment Setup
- Checked system and found `winget` available
- Installed **Ruby 3.3.11** with DevKit via winget
- Installed **Jekyll 4.4.1** and **Bundler 4.0.10** via gem

### 2. Jekyll Site Creation
- Scaffolded a new Jekyll site in `C:\Users\Lenovo\Caladrius-dev`
- Started the local dev server at `http://localhost:4000`

### 3. Content Added
- Copied `Caladrius Homepage V3 _standalone_` → `caladrius-homepage.html` (Version 1)
- Copied `caladrius-homepage-final` → `caladrius-homepage-v2.html` (Version 2)
- Updated the homepage (`index.markdown`) with links to both versions
- Added the April 7, 2026 article *"Beyond NHCX: Global Claims Exchange Models"* as a blog post
- Created a `/blog/` page and linked it from the homepage

### 4. GitHub Setup
- Connected the repo to `https://github.com/Sharonwatson-Sharon/Caladrius-dev.git`
- Authenticated using a Personal Access Token
- Created a GitHub Actions workflow (`.github/workflows/jekyll.yml`) for automated deployment
- Fixed a `Gemfile.lock` platform issue (added `x86_64-linux` for the Ubuntu runner)

### 5. GitHub Pages
- Site is live at: **https://sharonwatson-sharon.github.io/Caladrius-dev/**
- Every push to `main` automatically rebuilds and redeploys the site

---

## Running Locally

```bash
bundle exec jekyll serve
```

Then visit `http://localhost:4000` in your browser.

---

## Project Structure

```
├── _posts/                  # Blog articles
├── .github/workflows/       # GitHub Actions deployment workflow
├── _config.yml              # Jekyll site configuration
├── index.markdown           # Homepage with links to both versions
├── blog.markdown            # Blog listing page
├── about.markdown           # About page
├── caladrius-homepage.html  # Homepage Version 1
├── caladrius-homepage-v2.html # Homepage Version 2
└── Gemfile                  # Ruby gem dependencies
```
