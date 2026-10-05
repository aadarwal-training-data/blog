# blog

Technical notes by Aadarsh Agarwal, written in [Quarto](https://quarto.org)
and published at <https://aadarwal-training-data.github.io/blog/>.

## Write a post

Create `posts/<slug>/index.qmd`:

```yaml
---
title: "Title"
description: "One line for the listing."
date: 2026-10-05
---
```

Push to `main`. GitHub Actions renders the site and deploys it to GitHub Pages.

## Preview locally

```bash
quarto preview
```

Posts with executable code are frozen (`_freeze/`): render them locally with
`quarto render posts/<slug>/index.qmd` and commit `_freeze/` with the post, so
CI never has to run the code.
