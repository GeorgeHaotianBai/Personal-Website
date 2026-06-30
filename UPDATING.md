# Updating the website

The site keeps content in small YAML and Markdown files. GitHub Pages rebuilds the public site after changes reach the `main` branch.

## Add or edit a paper

Edit `data/papers.yaml`. Copy an existing paper entry and update its title, authors, status, abstract, image, and links. Upload the figure to `static/images/`. Upload a paper PDF to `static/files/` and set `pdf: "files/your-paper.pdf"`.

## Update the biography

Edit `content/_index.md`. The name, program, email address, and social link live in `hugo.yaml` and `layouts/index.html`.

## Add teaching

Edit `data/teaching.yaml` and follow the existing field structure.

## Add a work in progress or data project

Edit `data/work_in_progress.yaml` or `data/projects.yaml`.

## Update reading-group materials

Edit `data/reading_groups.yaml`. Each season contains a list under `slides`.

## Add a blog later

Create `content/blog/your-post/index.md` with this structure:

```yaml
---
title: "Post title"
date: 2026-01-15
description: "One-sentence summary."
tags: ["innovation"]
---

Write the post here.
```

## Add a CV later

Upload the file as `static/files/cv.pdf`. Add a CV menu item in `hugo.yaml` that points to `/files/cv.pdf`.

## Add a photo later

Upload the image as `static/images/photo.jpg`. The current hero intentionally uses a text-only composition, so adding a portrait also requires a small layout update.

## Change a paper's status

Change the `status` field in `data/papers.yaml`. Add a `venue` field if a paper is published. A future job-market paper can use `job_market_paper: true` and receive a dedicated template treatment.
