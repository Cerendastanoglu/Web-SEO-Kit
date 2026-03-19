# Structured Data (JSON-LD) - Copy Notes

These snippets are JSON-LD meant for:

```html
<script type="application/ld+json">
  { ...your JSON here... }
</script>
```

Put them in your page’s `<head>` (or right after opening `<body>`), and make sure:

- The content you describe matches what’s visible on the page.
- URLs/images are absolute and publicly reachable.
- You do not include duplicate conflicting structured data.

## Quick mapping

- `SCHEMA-ORGANIZATION.jsonld` -> site/company identity (`Organization`)
- `SCHEMA-ARTICLE.jsonld` -> blog posts/articles (`Article`)
- `SCHEMA-FAQ.jsonld` -> FAQ sections (`FAQPage`)

