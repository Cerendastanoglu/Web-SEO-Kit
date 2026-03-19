# Comprehensive SEO Checklist (Copy-Everywhere)

This checklist consolidates upstream requirements and recommendations from:

- `marcobiedermann/search-engine-optimization` (implementation bible)
- `flowforfrank/seo-checklist` (technical/on-site/off-site requirements)
- `joshbuchea/HEAD` (SEO-relevant HTML `<head>` elements)

Use it as:

- A per-page gate (you can check items while implementing a template or writing content)
- A site-wide gate (you can do a full audit before launch)

---

## 0) Plan (before you implement)

- [ ] Define the target keyword / keyphrase for the page
- [ ] Write a unique page title (aim ~50-60 chars)
- [ ] Write a unique meta description (aim ~120-160 chars)
- [ ] Decide the canonical URL for the page
- [ ] If you have multiple languages/regions, decide `hreflang` mappings
- [ ] Ensure the page has a real purpose (not thin/duplicated content)

---

## 1) Technical SEO (site + template requirements)

- [ ] Identify crawl/indexing issues (Search Console Coverage)
- [ ] Use URL inspection to confirm Google can index the page
- [ ] No broken links (avoid pages returning 4xx/5xx where possible)
- [ ] No blocked pages (no accidental `noindex`/`X-Robots-Tag`/robots blocks)
- [ ] Optimized 404 page (useful message + link to home + navigation/search)
- [ ] Served over HTTPS (and redirect HTTP -> HTTPS)
- [ ] Mobile friendly (test with Google’s Mobile-Friendly Test or Lighthouse)

### Page speed efficiency / Web performance

- [ ] Browser caching enabled for static assets (images, fonts, CSS/JS)
- [ ] Compression enabled (gzip or brotli)
- [ ] Resources minified (HTML/CSS/JS)
- [ ] Images and fonts optimized (size, format, fewer variants)

### Robots + sitemaps

- [ ] `robots.txt` is valid and correctly configured
- [ ] `sitemap.xml` exists and is valid
- [ ] Sitemap includes important pages (only as needed)

### Structured data

- [ ] Page has valid structured data (test with Structured Data Testing Tool)
- [ ] Structured data matches the page content (avoid spammy/incorrect markup)

### Core Web Vitals (UX metrics)

- [ ] LCP: good (<= 2.5s is a common threshold)
- [ ] FID: good (<= 100ms is a common threshold)
- [ ] CLS: good (<= 0.1 is a common threshold)

---

## 2) On-page SEO (template + each page)

### Meta information (head)

- [ ] Meta description exists and is unique
- [ ] Viewport meta tag exists
- [ ] Open Graph tags exist (OG title/type/url/image/description)
- [ ] Document uses HTML5 (`<!doctype html>`)
- [ ] Page includes a `<title>` tag
- [ ] `hreflang` is correct (when applicable)
- [ ] Favicon exists
- [ ] Canonical is correct (prevents duplicate content issues)

### Document structure & semantics

- [ ] Use SEO-friendly URLs (letters/numbers/dashes/underscores; no messy parameters)
- [ ] Headings follow hierarchy (H1 then H2 then H3; no skipped order)
- [ ] Image elements have `alt` attributes
- [ ] Images include `width` and `height` to prevent layout shift (where applicable)
- [ ] Off-screen images use `loading="lazy"` (avoid lazy-loading above-the-fold)
- [ ] Font sizes are legible (avoid tiny text < 12px)
- [ ] Tap targets are appropriately sized (around 48x48px) and not overlapping
- [ ] Avoid plugin-based content (`embed/object/applet` etc.); use compatible HTML/CSS/JS

### Accessibility + indexing safety

- [ ] Use semantic layout (prefer `div`s over `tables` for layout)
- [ ] Implement proper 403/404 behaviors (access denied + page not found)
- [ ] If you moved content, redirect with 301 (avoid excessive redirects like 302 chains)
- [ ] For paginated series, implement `rel="next"` / `rel="prev"`

---

## 3) Content requirements (writing + publishing)

### Keyword / keyphrase usage

- [ ] Keyphrase appears in the title
- [ ] Keyphrase appears in at least one H1/H2 subheading
- [ ] Keyphrase appears in the first paragraph
- [ ] Keyphrase appears in the slug (SEO-friendly URL)
- [ ] Keyphrase appears in meta description
- [ ] Keyphrase appears in image `alt` where it truly describes the image
- [ ] Keyword density is sensible (commonly referenced target: ~1-3%)
- [ ] Avoid duplicating the same keyphrase strategy across unrelated pages

### Structure + readability

- [ ] Use strong, clear headings (aim <= ~70 chars in many cases)
- [ ] Subheading distribution helps scanning (especially for long text)
- [ ] Paragraphs are reasonably short (commonly ~200 words or less)
- [ ] Sentences are not overly long (split if readability suffers)
- [ ] Text length is sufficient for the topic (often 300+ words; for competitive SEO commonly 1000+)
- [ ] Use transition words naturally (`and/but/so/because`) to improve flow
- [ ] Prefer active voice when possible
- [ ] Use `strong` tags to highlight targeted keyword phrases (sparingly and naturally)

### Uniqueness + freshness

- [ ] Content is unique (avoid copied/duplicated content)
- [ ] Update important pages periodically (freshness/maintenance helps)
- [ ] Avoid legacy Flash/Flash-like pages (use modern HTML5 media)

---

## 4) Images, videos, and media SEO

### Images

- [ ] Alt text describes the image content (often ~60-70 chars target for concise descriptions)
- [ ] Descriptive file names (short and meaningful)
- [ ] Use responsive images (serve appropriate sizes per viewport)
- [ ] Keep image file size low (compress; use modern formats when possible)

### Videos

- [ ] Use HTML5-compatible video embeds
- [ ] Include controls (when using self-hosted video)
- [ ] Provide transcriptions for indexing and accessibility
- [ ] Ensure videos are playable (avoid unplayable/blocked embeds)

---

## 5) Links (internal + outbound + rel rules)

- [ ] Add internal links throughout the site (help hierarchy and navigation)
- [ ] Internal linking prioritizes cornerstone/important pages
- [ ] Use descriptive link text (avoid “click here”)
- [ ] External/outbound links support the page topic (only when helpful)
- [ ] Apply `rel="nofollow"` to external links when appropriate (e.g., spam/risky destinations)

---

## 6) Off-site SEO (link building)

- [ ] Build backlinks ethically (quality > quantity)
- [ ] Avoid spam signals (too many links for a thin/irrelevant page)
- [ ] Prefer good link types:
  - [ ] Editorial links
  - [ ] Guest posting (quality-focused)
  - [ ] Niche-relevant directories/resources
  - [ ] Links from high-authority sites
- [ ] Avoid or disavow harmful link types:
  - [ ] Paid links / link schemes
  - [ ] Spammy comments or low-quality user-generated spam
  - [ ] Unrelated foreign sites
  - [ ] Links from dead/invalid domains
- [ ] Use `rel` attributes correctly on outbound links (understand `nofollow` semantics)

---

## 7) Social metadata (per page)

- [ ] OG tags are accurate and unique per page
- [ ] Twitter card tags are present and match your preview assets
- [ ] OG/Twitter images are publicly reachable and valid

---

## 8) Launch & verification (last mile)

- [ ] Validate `robots.txt` and `sitemap.xml`
- [ ] Validate structured data (testing + linting tools)
- [ ] Run Lighthouse for performance/accessibility/SEO checks
- [ ] Confirm indexing in Search Console (URL Inspection)

