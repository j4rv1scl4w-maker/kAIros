# Kairos — Nicolò Marana's blog

Personal blog on **tech, AI and software development**. Static site built with
[Jekyll](https://jekyllrb.com/) and published for free with **GitHub Pages**.

🔗 **Site:** https://j4rv1scl4w-maker.github.io/kAIros

---

## How to publish an article

Each article is a single Markdown file inside the `_posts/` folder.

### 1. File name

It must follow **exactly** this format:

```
_posts/YEAR-MONTH-DAY-title-with-dashes.md
```

Example: `_posts/2026-07-15-the-future-of-ai-agents.md`

### 2. File content

At the top goes the header (the "front matter") between `---`, then the text:

```markdown
---
title: "Article title"
date: 2026-07-15
tags: [ai, agents, software]
description: "A 1-2 sentence summary shown on Google and when you share the link on social."
---

Write the body of the article here in **Markdown**.

## A subheading

Plain text, lists, links, images, code... all supported.
```

| Field         | Required | Notes                                              |
|---------------|----------|----------------------------------------------------|
| `title`       | ✅       | Article title                                      |
| `date`        | ✅       | Format `YYYY-MM-DD` (must match the file name)     |
| `tags`        | ❌       | List of keywords in square brackets                |
| `description` | ❌ (recommended) | Summary for SEO and social previews        |

### 3. Publish

Save the file, commit and push. GitHub Pages rebuilds the site by itself in
1-2 minutes. **No build command needed.**

> 💡 Alternatively, just hand the title and text to Nicolò (or the assistant):
> the file gets created and published for you.

---

## Quick Markdown reminder

```markdown
## Big heading         ### Medium heading
**bold**               *italic*
[link text](https://example.com)
![description](path/image.jpg)
- bullet point         1. numbered list
> quote                `inline code`
```

---

## SEO and indexing (already configured)

- ✅ Automatic **sitemap** (`/sitemap.xml`)
- ✅ **Meta tags** Open Graph + Twitter Card on every page
- ✅ **RSS feed** (`/feed.xml`)
- ✅ **robots.txt** inviting search engines to index everything

To speed up indexing on Google: register the site on
[Google Search Console](https://search.google.com/search-console) and submit
the sitemap URL.

---

## Local development (optional)

```bash
bundle install
bundle exec jekyll serve
# open http://localhost:4000/kAIros
```

---

## Project structure

```
_config.yml          Site configuration
_posts/              👈 The articles (one Markdown file each)
_layouts/            HTML page templates
_includes/           Reusable header, footer, head
assets/css/          Styling (dark/tech, mobile-first)
index.html           Home page with the article list
about.md             "About" page
```
