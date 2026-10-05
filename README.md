# blog

Technical notes by Aadarsh Agarwal, written in [Quarto](https://quarto.org)
and published at <https://aadarwal-training-data.github.io/blog/>.

## Write a post

```bash
cp -r posts/_template posts/<slug>
```

Edit `posts/<slug>/index.qmd`, then delete its `draft: true` line to publish.
Push to `main`; GitHub Actions renders the site and deploys it to GitHub Pages.
Also add the post to the `#blog` list on www.aadarwal.com (`index.html` in the
`aadarshagarwal.com` repo).

## Preview locally

```bash
quarto preview
```

Posts with executable code are frozen (`_freeze/`): render them locally with
`quarto render posts/<slug>/index.qmd` and commit `_freeze/` with the post, so
CI never has to run the code.
