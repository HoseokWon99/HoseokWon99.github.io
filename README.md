# HoseokWon99.github.io

Hugo-powered GitHub Pages blog with English/Korean routes, Markdown posts, KaTeX math rendering, categories, tags, and Pagefind full-text search.

**Link**: [HoseokWon99.github.io](https://HoseokWon99.github.io)

## Local Development

Install dependencies once:

```sh
npm install
```

Run the development server:

```sh
npm run dev
```

Build the production site:

```sh
npm run build
```

Build the site and generate the Pagefind search index:

```sh
npm run build:search
```

## Writing Posts

English posts live in `content/en/posts/`.

Korean posts live in `content/ko/posts/`.

Use Markdown front matter like this:

```yaml
---
title: "Post title"
date: 2026-05-03
description: "Short search and listing summary."
contentLang: "en"
categories: ["Blog"]
tags: ["hugo", "math"]
draft: false
math: true
translationKey: "shared-post-key"
---
```

Set `math: true` only on posts that use LaTeX formulas. Inline math uses `$...$`, and block math uses `$$...$$`.

Use the same `translationKey` on English and Korean versions of the same post to enable language switching.

## URLs

- `/` redirects to `/en/`
- `/en/posts/<slug>/`
- `/ko/posts/<slug>/`
- `/en/search/` and `/ko/search/`
- `/en/categories/` and `/ko/categories/`
- `/en/tags/` and `/ko/tags/`

## Deployment

The GitHub Actions workflow in `.github/workflows/pages.yml` builds Hugo, generates the Pagefind index, uploads `public/`, and deploys it to GitHub Pages on pushes to `main`.
