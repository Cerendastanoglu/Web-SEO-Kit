# Web SEO Kit

Copy this folder into any website project to get:

- A comprehensive SEO checklist (technical + on-page + content + off-site)
- Copy-ready HTML `<head>` snippets
- `robots.txt` + `sitemap.xml` templates
- A curated list of SEO tools
- Source attribution for the materials this kit is based on

## How to use (fast)

1. Paste `web-seo-kit/snippets/HEAD.html` into your templates.
2. Create `robots.txt` and `sitemap.xml` from:
   - `web-seo-kit/snippets/ROBOTS.txt`
   - `web-seo-kit/snippets/SITEMAP.xml`
3. Use `web-seo-kit/CHECKLIST.md` as your “page + site” SEO gate.
4. When you need tools, open `web-seo-kit/TOOLS.md`.

## What’s included

- `CHECKLIST.md`: consolidated requirements checklist pulled from:
  - `marcobiedermann/search-engine-optimization`
  - `flowforfrank/seo-checklist`
  - `joshbuchea/HEAD` (as HTML `<head>` requirements)
  - `teles/awesome-seo` + `serpapi/awesome-seo-tools` (as an SEO tooling index)
- `SOURCES.md`: links + attribution notes for each upstream repo.
- `vendor/ultimate-seo-checklist/`: full folder-by-folder checklist database (offline reference).

## Next additions (optional)

If you want this to be even more “copy-everywhere”, tell me your stack:

- Plain HTML (no framework)
- React / Next.js
- Vue / Nuxt
- SvelteKit
- WordPress
- Other

Then I’ll generate stack-specific templates (example: `next/head`, `app/metadata`, WordPress plugin settings, etc.).

