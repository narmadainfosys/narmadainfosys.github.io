# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a GitHub Pages site for Narmada Infosys, a software consultancy company. The repository contains:
- A main single-page portfolio website (Bootstrap-based)
- A Jekyll blog subdirectory at `/blog`

## Architecture

### Main Site (Root)
- **Framework**: Bootstrap 3 + jQuery
- **Structure**: Single-page application in `index.html`
- **Sections**: Services, Technology Portfolio, Work Timeline, Team, Contact
- **Assets**:
  - `/css` - Bootstrap and custom agency theme styles
  - `/js` - jQuery, Bootstrap, custom interactions
  - `/img` - Images for portfolio, team, and branding
  - `/font-awesome` - Icon library
  - `/fonts` - Glyphicons fonts

### Blog (blog/)
- **Framework**: Jekyll 3.6.2 with Minima theme
- **Config**: `blog/_config.yml`
- **Posts**: `blog/_posts/` (Markdown format: YYYY-MM-DD-title.markdown)
- **Build**: Jekyll generates static site to `blog/_site/`

## Key Commands

### Jekyll Blog Development

```bash
# Navigate to blog directory
cd blog

# Install dependencies
bundle install

# Serve blog locally (http://localhost:4000/blog)
bundle exec jekyll serve

# Build static site
bundle exec jekyll build
```

### Main Site

The main site is static HTML/CSS/JS. Simply open `index.html` in a browser or serve with any web server:

```bash
# Using Python 3
python3 -m http.server 8000

# Using Python 2
python -m SimpleHTTPServer 8000
```

## Deployment

This is a GitHub Pages site. Changes pushed to the `master` branch are automatically deployed to `narmadainfosys.github.io`.

- Main site is served from root
- Blog is served from `/blog` subdirectory

## Important Notes

- **Branch**: Main branch is `master` (not `main`)
- **Blog baseurl**: Blog is configured with baseurl `/blog` in `_config.yml`
- **No build process**: Main site has no build tooling (no npm/webpack)
- **Contact form**: Currently displays email only (NARMADAINFOSYS@MAIL.COM)
- **HubSpot**: Analytics tracking enabled via embed code in index.html:3925207

## Content Structure

### Team Members (index.html:319-363)
- Bishisht Bhatta - Linux, Python, Ruby, Rails, DevOps
- Sagar Pant - Marketing/CFO
- Amit Kumar - Android, Java, WordPress

### Technology Stack Showcased
- Bootstrap, Rails, Django, Heroku, AWS, Linux

## File Locations

- Main landing page: `/index.html`
- Blog configuration: `/blog/_config.yml`
- Blog posts: `/blog/_posts/`
- Team images: `/img/team/`
- Portfolio images: `/img/portfolio/`
