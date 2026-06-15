---
description: Optimize a page's title, meta description, headings, and content for a target keyword. Auto-activates when the user asks to optimize a page for SEO, improve rankings, rewrite a title tag or meta description, or fix on-page SEO.
---

Optimize on-page SEO for: $ARGUMENTS

## Instructions

Parse $ARGUMENTS to identify:
- A **URL** to fetch (use WebFetch) — OR —
- A **target keyword** — OR —
- Both a URL and a target keyword (e.g. "https://example.com for 'seo audit tool'")

If a URL is provided, fetch the page and extract current title, meta description, H1, and first 200 words.
If a target keyword is not specified, infer it from the page content.

---

## What to optimize

### 1. Title tag
- 50–60 characters
- Primary keyword near the start
- Brand name at the end separated by ` | ` or ` – `
- Compelling and click-worthy, not keyword-stuffed

Output: **Current title** → **Optimized title** (with character count)

### 2. Meta description
- 120–155 characters
- Contains primary keyword and a secondary variation
- Has a clear value proposition or call to action
- Written for humans, not bots

Output: **Current description** → **Optimized description** (with character count)

### 3. H1
- Exactly one H1 per page
- Contains the primary keyword naturally
- Different from the title tag (complementary, not identical)

Output: **Current H1** → **Optimized H1**

### 4. H2 structure
- Suggest 4–6 H2s that cover the topic comprehensively
- Each H2 should target a supporting keyword or subtopic
- H2s should follow a logical reading flow

Output: Suggested H2 list

### 5. First paragraph
- Primary keyword in the first 100 words
- Sets up the page topic clearly for both users and crawlers
- Should answer the search intent immediately

Output: Rewritten first paragraph (if needed)

### 6. Internal linking suggestions
- Suggest 2–3 anchor text phrases from the page content that could link to related pages
- Format: `"[anchor text]"` → link to a page about [topic]

---

## Output format

Present each element as a before/after comparison with a one-line explanation of what changed and why. End with a **Priority order** — which change will have the highest ranking impact first.
