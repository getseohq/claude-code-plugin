---
description: Generate JSON-LD structured data / schema markup ready to paste into a webpage. Auto-activates when the user asks for schema markup, structured data, JSON-LD, rich results, or schema.org markup.
---

Generate ready-to-paste JSON-LD structured data for: $ARGUMENTS

## Instructions

If the user provides a URL, fetch it with WebFetch and infer the schema type from the page content. If they describe the page or schema type in $ARGUMENTS, use that directly. If neither is clear, ask: "What type of page or content do you need schema for?"

### Supported schema types

- **Article** — blog posts, news articles, how-to guides
- **Product** — e-commerce product pages
- **FAQ** — pages with questions and answers
- **HowTo** — step-by-step guides
- **LocalBusiness** — brick-and-mortar business pages
- **BreadcrumbList** — navigation breadcrumbs
- **WebSite** — homepage with sitelinks search box
- **Person** — author or personal profile pages
- **Organization** — company/brand pages
- **Event** — events with date, location, and ticket info
- **Review / AggregateRating** — review pages or product ratings
- **VideoObject** — pages with embedded videos
- **Recipe** — cooking recipe pages
- **JobPosting** — job listing pages
- **Course** — online course or educational content

### Steps

1. Identify the correct schema type(s) for the page — a page can have multiple JSON-LD blocks
2. Extract or infer all required and recommended properties
3. Output valid JSON-LD wrapped in `<script>` tags, ready to paste into `<head>`
4. After the code block, list:
   - Which properties are **required** by Google (and are present)
   - Which **recommended** properties are missing and what to fill in
   - A link to test it: `https://search.google.com/test/rich-results`

### Quality rules
- Use `@context: "https://schema.org"` (not http)
- Dates in ISO 8601 format (`2024-03-15` or `2024-03-15T09:00:00+00:00`)
- Images must be absolute URLs
- Never invent data — use placeholder comments like `"// ADD: your phone number"` for missing info
- Prefer `@type` arrays when a page fits multiple types (e.g. `["Article", "NewsArticle"]`)

Output the schema block first, then the property checklist.
