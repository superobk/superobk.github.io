# Homepage Content Update Guide

The homepage is composed from the Markdown files in `_sections/`. Edit one file to update one visible section; the layout and navigation are generated automatically from its front matter.

## Update A Section

1. Edit the matching file in `_sections/`.
2. Keep `title`, `nav_label`, `slug`, `order`, `status`, `show_in_nav`, `image`, and `image_alt` in its front matter.
3. Set `status: current` when the content is confirmed. Keep `status: draft` to retain the visible `To be continued.` marker.
4. Use only public, durable links and media. Do not add customer names, internal paths, private data, exact deployment configuration, or unpublished research results.

## Add A Project

Add the following entry to `_sections/selected-work.md` after the existing public items:

```markdown
### Project Name

One short public description of the problem, contribution, and outcome. Link only to stable public material.

- [Project page](https://example.com/)
- [Code](https://github.com/example/project)
```

For a visual, place a public image in `assets/` and set `image: /assets/your-image.png` in that section's front matter. Keep `image_alt` descriptive.

## Preview And Publish

```bash
# Optional local preview, after installing Jekyll and Bundler locally:
jekyll serve
git diff --check
rg -n -i 'NVP|community|ObjectVLN|HomeBot|OmniVLA|/Users/bou|Mobile Documents|private dataset|customer name' .
git add _config.yml index.md _layouts _sections assets CONTENT-UPDATE-GUIDE.md
git commit -m "Refresh personal homepage"
git push origin main
```

GitHub Pages publishes from `main`. After deployment, verify `https://superobk.github.io/?v=<commit-sha>` and confirm that the edited navigation anchor works.
