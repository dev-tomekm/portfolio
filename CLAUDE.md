# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static single-page portfolio/CV site for Tomasz Michniewicz. No build system, no bundler, no package manager — just a single `index.html` with external CDN dependencies.

## Development

Serve locally with VS Code Live Server on port 5501 (configured in `.vscode/settings.json`).

## Architecture

- **Single file**: All markup lives in `index.html` (~1060 lines)
- **CSS framework**: Tailwind CSS via Preline UI CDN (`preline.co/assets/css/main.min.css`)
- **JS**: Preline UI JS from jsDelivr CDN for interactive components (collapse nav, theme toggle)
- **Dark mode**: Uses `localStorage` key `hs_theme` with Preline's dark mode classes
- **Sections** (in order): Header/Nav, Hero image grid, About/Bio, Skills timeline, Testimonials, Projects, Contact form, Footer
- **Assets**: `assets/images/avatar.jpg` — most other images are Unsplash CDN URLs
