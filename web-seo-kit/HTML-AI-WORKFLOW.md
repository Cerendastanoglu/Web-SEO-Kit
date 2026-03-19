# HTML Project AI Workflow (Plain HTML/CSS/JS)

Yes, we can do that in Cursor: you open your website repo here, and you tell me what page you’re building; then you copy/paste your HTML (or point me to the file), and I’ll implement the SEO changes directly in your project.

## What I can implement

- Update `<head>` tags:
  - `title`, `meta name="description"`
  - `link rel="canonical"`
  - `meta name="robots"` (+ `googlebot` optional)
  - Open Graph + Twitter card tags
  - Hreflang (if you have multiple languages)
- Add structured data:
  - Organization / Article / FAQ JSON-LD (using your content)
- Add/adjust `robots.txt` and `sitemap.xml` templates (and ensure they match your URLs)

## What you need to provide (fast checklist)

1. The target page:
   - file path (example: `site/about.html`) OR paste the HTML from the page
2. Site basics:
   - site name
   - base URL (example: `https://example.com`)
3. Page specifics:
   - page title
   - meta description
   - canonical URL
   - OG/Twitter image URL (publicly reachable)
   - primary topic + a few keywords (optional but helpful)
4. If you want JSON-LD:
   - Organization info (name, logo, social links)
   - Article info OR FAQ questions/answers

## Copy/paste prompt you can use for me

Paste this and fill in the brackets:

```text
You are editing a plain HTML/CSS/JS website.

Task:
Update the SEO for this page by editing the existing HTML file in my repo.

File path:
[PASTE FILE PATH]

Site:
- Site name: [YOUR_SITE_NAME]
- Base URL: [https://example.com]

Page:
- Page title: [YOUR_PAGE_TITLE]
- Meta description: [YOUR_UNIQUE_PAGE_DESCRIPTION]
- Canonical: [https://example.com/your-page/]
- OG image: [https://example.com/path/to/og-image.jpg]

Structured data:
Use [Organization] / [Article] / [FAQ] JSON-LD.
If Article: provide headline + dates + image URL.
If FAQ: provide 3-6 questions and answers.

Rules:
- Keep everything else as-is.
- Only modify what’s needed in <head> (and add JSON-LD script if requested).
- Ensure JSON-LD values match the visible content.
```

## Practical flow in Cursor

1. Open your project folder in Cursor
2. Tell me which file is the page you’re working on
3. Paste the page HTML (if you don’t want to share the file path)
4. Use the prompt above and I’ll return the exact edits

