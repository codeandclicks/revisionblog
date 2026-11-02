# Revision Blog

Revision Blog is a static blog built with [Hexo](https://hexo.io/) and the Landscape theme. Posts are written in Markdown and published as static files.

## Features

- Markdown-based blog posts with categories and tags.
- Generated home page, archives, categories, and tag pages.
- Landscape theme with EJS templates, Markdown rendering, and Stylus styles.

## Technology

- Node.js and npm
- Hexo 8
- Hexo Landscape theme
- Hexo generators for index, archives, categories, and tags

## Run locally

Requires Node.js (18 or newer) and npm.

```bash
npm install
npm run server
```

Open the local address printed by Hexo (usually http://localhost:4000). The server watches for changes while you work.

## Create a post

Add a Markdown file under `source/_posts/`, for example `source/_posts/my-post.md`:

```markdown
---
title: My Post
date: 2026-11-02 12:00:00
categories:
  - Updates
tags:
  - news
---

Write your post here.
```

## Build the site

```bash
npm run build
```

Hexo generates the static site in `public/`. Use `npm run clean` to remove generated output.

## Configuration and deployment

Edit `_config.yml` to set the site title, description, author, URL, language, and theme options. The checked-in configuration currently has starter values; update them before publishing. Deployment is not configured yet (`deploy.type` is empty), so set up a Hexo deployer and destination before using `npm run deploy`.

## Project structure

```text
_config.yml          Hexo site configuration
source/_posts/       Markdown blog posts
themes/              Optional local themes
package.json          Hexo scripts and dependencies
public/               Generated site output (after build)
```
