# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Blacksmith is a landing page for a custom AI consultancy targeting small/independent retail businesses (jewelry stores, convenience stores, liquor stores, wholesalers). The site promotes AI-powered tools (inventory management, web storefronts, product listing) built by founder Ahad Ali.

## Architecture

This is a **single-file static site** — everything lives in `index.html`:
- All CSS is inline in a `<style>` block (no external stylesheets beyond Google Fonts)
- No JavaScript
- No build step, bundler, or framework
- Deployed to Vercel as a static site (auto-deploys from GitHub on push to `main`)

## Deployment

- **Hosting**: Vercel (linked to GitHub repo `ahadali1031/blacksmith-landing`)
- **URL**: https://blacksmith-landing.vercel.app
- Push to `main` triggers automatic deployment — no build command needed

## Design System

CSS custom properties defined in `:root`:
- `--cream`, `--warm-white`, `--charcoal`, `--gold`, `--gold-light`, `--gold-pale`, `--stone`, `--stone-light`, `--rust`, `--green`

Typography:
- Headings: `Cormorant Garamond` (serif)
- Body: `DM Sans` (sans-serif)
- Labels/mono elements: `DM Mono` (monospace)

## Page Sections

nav → hero (two-column) → proof-strip → how-it-works → who-this-is-for → about → CTA → footer

All CTAs link to: `https://calendly.com/ahad-ali1031/30min`
