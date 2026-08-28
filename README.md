# Benson.O Homepage

This is the GitHub Pages source for [superobk.github.io](https://superobk.github.io/). It uses native Jekyll collections and a custom layout; no frontend framework or non-standard GitHub Pages plugin is required.

## Structure

- `index.md`: selects the homepage layout.
- `_layouts/profile.html`: navigation, profile sidebar, section renderer, and footer.
- `_sections/*.md`: one public homepage section per Markdown file.
- `assets/css/profile.css`: responsive visual system.
- `assets/`: public images used by the page.
- `CONTENT-UPDATE-GUIDE.md`: the routine for editing, checking, and publishing content.

The page includes `About`, `Focus`, `Projects`, `News`, `Experience`, `Publications`, `Life`, and `Contact`. A section with `status: draft` keeps its title in navigation and visibly displays `To be continued.` until its public content is ready.

## Publish

```bash
git diff --check
git add _config.yml index.md _layouts _sections assets CONTENT-UPDATE-GUIDE.md README.md
git commit -m "Refresh personal homepage"
git push origin main
```

GitHub Pages publishes the `main` branch at `https://superobk.github.io/`.
