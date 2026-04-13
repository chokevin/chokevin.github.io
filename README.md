# chokevin.github.io

Minimal personal blog for GitHub Pages.

## Stack

- GitHub Pages
- Jekyll (built in by GitHub Pages for user sites)

## How publishing works

1. Edit or add files in this repo.
2. Push to `master`.
3. GitHub Pages publishes to `https://chokevin.github.io`.

## Create a new post

1. Add a file to `_posts` named `YYYY-MM-DD-title.md`.
2. Use this front matter:

```md
---
layout: post
title: "Post title"
date: 2026-04-13 10:00:00 -0700
---
```

3. Write your content in Markdown, commit, and push.

## Key files

- `_config.yml` — site settings
- `_layouts/default.html` — site layout and styling
- `_layouts/post.html` — blog post layout
- `index.html` — home page with latest post list
- `about.md` — about page

## Azure migration (phase 2)

When Azure account access is stable, migrate to Azure Static Web Apps by:

1. Creating a new Static Web App resource.
2. Connecting this repo/branch in the deployment wizard.
3. Validating preview and production URLs.
4. Cutting over DNS (if using a custom domain) with rollback notes.

