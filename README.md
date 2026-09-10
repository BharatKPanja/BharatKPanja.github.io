# BharatKpanja.github.io

Personal hub for Bharat Panja — served at **https://bharatkpanja.github.io**.
Built with [Jekyll](https://jekyllrb.com/) and the
[Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) remote theme.

## Layout

| Path | What it is |
|---|---|
| `_config.yml` | Site settings, theme, author sidebar, collections |
| `index.md` | Home / landing page |
| `_pages/about.md` | About — the career story |
| `_pages/articles.md` | Articles listing (lists `_posts`) |
| `_pages/topics.md` | Topics listing (lists `_topics`) |
| `_pages/projects.md` | Projects listing (lists `_projects`) |
| `_posts/` | Articles & notes — `YYYY-MM-DD-title.md` |
| `_topics/` | Deep-dive topic pages |
| `_projects/` | Selected work / case studies |
| `assets/images/` | Images, incl. `profile.jpg` for the avatar |
| `_data/navigation.yml` | Top navigation bar |

## How it scales

Each content type is its own **collection**. To add a new section later, create a
folder (e.g. `_talks`), register it under `collections:` in `_config.yml`, add a
listing page in `_pages/`, and add one line to `_data/navigation.yml`. No restructure.

### Add an article

Create `_posts/YYYY-MM-DD-your-title.md`:

```yaml
---
title: "Your title"
date: 2026-09-15
categories: [notes]
tags: [oci, migration]
excerpt: "One-line summary."
---
```

### Add a topic or project

Create a file in `_topics/` or `_projects/` with `title` and `excerpt` front matter.
It appears on the matching listing page automatically.

## Publishing

Push to GitHub, then **Settings → Pages → Build from the `master` branch**.
The site is live at the root URL within a minute or two.

## Local preview (optional)

```
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.
