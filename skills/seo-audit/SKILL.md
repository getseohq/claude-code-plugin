---
description: Audit a webpage for SEO issues and produce a scored report. Auto-activates when the user asks to audit a URL, check SEO, analyze a page for search optimization, or review on-page SEO factors.
---

Perform a comprehensive SEO audit of: $ARGUMENTS

## Steps

1. **Fetch the page** using the WebFetch tool. If no URL is provided, ask the user for one.

2. **Analyze these factors** and score each 0–100:

### Technical (25 pts)
- Title tag: present, 50–60 chars, contains primary keyword
- Meta description: present, 120–155 chars, compelling
- Canonical tag: present and correct
- robots meta: not accidentally blocking indexing
- Viewport meta: present (mobile-friendly)
- HTTPS: URL uses https://
- URL structure: short, descriptive, lowercase, hyphens not underscores

### On-Page (25 pts)
- H1: exactly one, contains primary keyword
- Heading hierarchy: logical H1 → H2 → H3 flow, no skipped levels
- First 100 words: contains primary keyword naturally
- Content length: estimate word count (longer is generally better for informational pages)
- Keyword density: not over-stuffed (< 3% for main keyword)
- Internal links: at least 2–3 links to other pages on the same domain

### Images (15 pts)
- Alt text: every `<img>` has descriptive alt text
- Descriptive filenames: not `IMG_1234.jpg`
- Lazy loading: images use `loading="lazy"` where appropriate

### Structured Data (15 pts)
- JSON-LD present: at least one schema block
- Schema type appropriate for page (Article, Product, FAQ, LocalBusiness, etc.)
- No validation errors visible in markup

### Content Quality (20 pts)
- Page has a clear topic and purpose
- Sufficient depth for the target keyword
- No obvious thin content or duplicate content signals
- Clear call to action

3. **Output a scored report** in this format:

---
## SEO Audit: [page title or URL]
**Overall Score: XX/100**

| Category | Score | Status |
|---|---|---|
| Technical | XX/25 | ✅ / ⚠️ / ❌ |
| On-Page | XX/25 | ✅ / ⚠️ / ❌ |
| Images | XX/15 | ✅ / ⚠️ / ❌ |
| Structured Data | XX/15 | ✅ / ⚠️ / ❌ |
| Content Quality | XX/20 | ✅ / ⚠️ / ❌ |

### Critical Issues (fix first)
- [list any 0-point items]

### Improvements
- [list specific, actionable fixes with expected impact]

### What's Working
- [list 2–3 things already done well]

### Quick Wins
- [list changes that take < 30 min and have high impact]
---

Be specific and actionable. Never say "improve your content" — say exactly what to change and why.
