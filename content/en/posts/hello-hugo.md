---
title: "Building a Technical Blog with Hugo"
date: 2026-05-03
description: "A first English post that verifies categories, tags, translations, and KaTeX rendering."
contentLang: "en"
categories: ["Blog"]
tags: ["hugo", "math", "search"]
draft: false
math: true
translationKey: "hello-hugo"
---

This post checks the core writing features for the blog: Markdown content, taxonomies, translated entries, search indexing, and formulas.

## Formula rendering

Inline math should render inside a sentence, such as $E = mc^2$.

Block math should render as a centered expression:

$$
\int_0^1 x^2\,dx = \frac{1}{3}
$$

## Search metadata

Pagefind should index the title, description, tags, categories, and the body text on this page. This makes the static site searchable without adding a server.
