# Minimal Academic Website

This repository is a minimal academic profile website for GitHub Pages.

The public site intentionally exposes only:

- Home
- Publications
- Group

## Edit Points

- Site title, URL, and general settings: `_config.yml`
- Home page bio and links: `_pages/about.md`
- Recent news: `_news/*.md`
- Publications: `_bibliography/papers.bib`
- Group page: `_pages/profiles.md`
- Minimal layout and styling: `_layouts/minimal.liquid`

## Local Build

This site uses the existing Jekyll/al-folio dependency stack.

```bash
bundle install
bundle exec jekyll serve
```

The current GitHub Actions deploy workflow uses Ruby 3.3.5.
