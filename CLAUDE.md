# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Backyard Brews — a single-page static website for a community-focused coffee shop in Petaling Jaya, Malaysia. The page is built with plain HTML and CSS (no frameworks, no build step).

## Key Files

- `index.html` — Main page (inline CSS, no external stylesheets)
- `index_ori.html` — Backup copy of the full original page
- `images/backyard-brews.png` — Brand hero image (vector-style illustration)

## Brand & Style

- **Brand tone**: Warm, cozy, community-focused
- **Colors**: Dark green (`#1c2e1f`), gold/amber (`#b8860b` / `#d4a843`), cream background (`#faf7f2`)
- **Fonts**: Playfair Display (headings), Inter (body) — both loaded from Google Fonts
- **Taglines**: "Good coffee. Good people. Great moments." / "See you in the backyard!"
- **Socials**: Instagram & TikTok — `@backyardbrews.my`

## Development

This is a plain static site with no build step. Just open `index.html` in a browser to preview.

```sh
open index.html
```

All styles are inline in the `<style>` block within `<head>`. No external CSS files.

## Mandatory Rules (AI must follow)

- **Git commits: never include Anthropic-related metadata** — no `Co-Authored-By: Claude`, no `noreply@anthropic.com`, no "🤖 Generated with..." lines, or any other Anthropic/Claude references in commit messages or PR bodies.
- The `.claude/settings.local.json` file uses a custom LLM provider (DeepSeek via API). Do not modify provider settings.
- Keep the brand color palette consistent when adding new sections.
- The site should remain responsive (mobile layout at 640px breakpoint).
