# BharatKpanja.github.io

Personal hub for Bharat Panja — served at **https://bharatkpanja.github.io**.
Built with [Jekyll](https://jekyllrb.com/) and the
[Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) remote theme.

## Layout

| Path | What it is |
|---|---|
| `_config.yml` | Site settings, theme, author sidebar |
| `index.md` | Home / landing page |
| `_pages/about.md` | About — the career story |
| `_pages/books.md` | Books |
| `_pages/inspiration.md` | Inspiration |
| `_pages/thoughts.md` | Thoughts |
| `_includes/footer.html` | Footer override (drops the theme credit) |
| `assets/images/` | Images, incl. `profile.jpg` for the avatar |
| `_data/navigation.yml` | Top navigation bar |

## Sections

The site has four pages — About, Books, Inspiration, Thoughts — each a single
Markdown file in `_pages/`. To add a new section, create a page there, give it a
`permalink`, and add one line to `_data/navigation.yml`.

### Add or edit a page

Each page in `_pages/` looks like:

```yaml
---
title: "Books"
permalink: /books/
author_profile: true
---

Your content here.
```

When any section grows into a long list of entries, it can be converted to a
Jekyll *collection* — not needed yet.

## Publishing

Push to GitHub, then **Settings → Pages → Build from the `master` branch**.
The site is live at the root URL within a minute or two.

## Local preview (optional)

```
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.
