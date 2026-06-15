# getseo.pro for Claude Code

Free AI-powered SEO toolkit that brings professional-grade search optimization directly into Claude Code. Audit pages, generate schema markup, cluster keywords, optimize content, and audit YouTube videos — all without leaving your editor.

Made by [getseo.pro](https://getseo.pro)

## Install

```
/plugin marketplace add getseohq/claude-code-plugin
/plugin install getseo
```

## Skills

### `/getseo:seo-audit <url>`
Full on-page and technical SEO audit with a scored report and prioritized action plan.

```
/getseo:seo-audit https://example.com
```

### `/getseo:schema-markup <url or description>`
Generate ready-to-paste JSON-LD structured data. Supports Article, Product, FAQ, HowTo, LocalBusiness, Event, and more.

```
/getseo:schema-markup https://example.com/product/widget
/getseo:schema-markup FAQ page about our pricing
```

### `/getseo:keyword-cluster <keywords>`
Group a keyword list by search intent (informational, commercial, transactional) and map each cluster to the right content type.

```
/getseo:keyword-cluster seo tool, seo audit, best seo software, free seo checker, seo audit tool
```

### `/getseo:on-page-seo <url> for "<keyword>"`
Optimize title tags, meta descriptions, H1, and content structure for a target keyword.

```
/getseo:on-page-seo https://example.com for "seo audit tool"
```

### `/getseo:youtube-audit <youtube-url>`
Audit a YouTube video using real data from the YouTube API — title, description, tags, and engagement scored with actionable fixes.

```
/getseo:youtube-audit https://youtube.com/watch?v=dQw4w9WgXcQ
```

### `/getseo:youtube-optimize <youtube-url or topic>`
Get optimized title options, a ready-to-paste description, and a full tag list for any YouTube video or topic.

```
/getseo:youtube-optimize https://youtube.com/watch?v=dQw4w9WgXcQ
/getseo:youtube-optimize how to do keyword research for beginners
```

## Agent

### `seo-auditor`
Deep-dive audit agent for full site analysis. Fetches multiple pages, identifies site-wide patterns, and produces a structured report with executive summary. Invoke it from `/agents` or ask naturally:

> "Run a full SEO audit of getseo.pro"

## Natural language

Skills activate automatically when you ask naturally:

- "Audit this page for SEO issues: example.com"
- "Generate schema markup for my product page"
- "Cluster these keywords by intent: [list]"
- "Optimize my title tag and meta description for 'seo tool'"
- "Audit my YouTube video: youtube.com/watch?v=..."
- "Optimize the title and tags for this YouTube video"

## About

[getseo.pro](https://getseo.pro) is an SEO analysis platform for developers and marketers. This Claude Code plugin brings the same analysis capabilities directly into your development workflow.

- Website: [getseo.pro](https://getseo.pro)
- Issues: [github.com/getseohq/claude-code-plugin/issues](https://github.com/getseohq/claude-code-plugin/issues)
