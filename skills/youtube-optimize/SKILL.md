---
description: Optimize a YouTube video's title, description, and tags for better search rankings. Auto-activates when the user asks to optimize a YouTube video, rewrite a YouTube title or description, improve YouTube tags, or get more YouTube views.
---

Optimize YouTube SEO for: $ARGUMENTS

## Instructions

Parse $ARGUMENTS to identify:
- A **YouTube URL** — run the audit first via the getseo.pro API, then optimize based on real scores
- A **title, description, or tags** pasted directly — optimize those
- A **topic or keyword** — generate optimized title, description, and tags from scratch

If a YouTube URL is provided, first call:
```bash
curl -s -X POST https://getseo.pro/api/v1/youtube \
  -H "Content-Type: application/json" \
  -d '{"url": "<VIDEO_URL>"}'
```
Use the real data to inform your optimizations.

---

## What to optimize

### 1. Title
Rules:
- 50–70 characters (never over 100)
- Primary keyword in the first 3 words where possible
- Include a number if it fits naturally
- Use a power word: How, Why, Best, Ultimate, Complete, Proven, Easy, Fast
- Format options that perform well: "How to X (Without Y)", "X Things About Y", "The Truth About X", "X vs Y: Which Is Better?"

Output: **Current title** → **3 optimized title options** (with character counts)

### 2. Description
Rules:
- First 150 characters must contain the primary keyword — this is what shows before "Show more"
- Total length: 500–1000 characters
- Include 3–5 natural keyword variations
- Add timestamps if the video has chapters (format: `0:00 Intro`)
- Add 3–5 hashtags at the end
- Include at least one link (channel, website, or related video)
- End with a call to action: subscribe, comment, or visit a link

Output: Full rewritten description ready to paste

### 3. Tags
Rules:
- 8–15 tags total
- Mix of: exact keyword, broad keyword, long-tail phrases (3+ words), channel name
- No tags over 127 characters
- First tag should be your exact primary keyword

Output: Comma-separated tag list ready to paste into YouTube Studio

### 4. Thumbnail recommendation
- Suggest a thumbnail concept based on the title and topic
- High-contrast colors, large readable text (3–4 words max), face if possible
- Format: describe the ideal thumbnail in 2–3 sentences

---

## Output format

Present as four clear sections: Title Options, Description, Tags, Thumbnail. Each section ready to copy-paste directly into YouTube Studio.

End with: "Run `/getseo:youtube-audit <url>` after updating to see your new score. Full history at https://getseo.pro"
