# Taco Bell Media

Purple-and-white, mid-2000s corporate news site, built with Jekyll for GitHub Pages.

## Publish
Add a Markdown file in `_posts/` named `YYYY-MM-DD-headline.md`:

```markdown
---
layout: post
title: "Your headline"
date: 2026-11-11 12:00:00 -0500
author: "Your name"
category: "Politics"
description: "A one-sentence summary of the report."
# Optional: image: "/assets/images/story-photo.jpg"
---

Your article text here.
```

The **NEWSWIRE** strip scrolls the latest eight headlines automatically. Hover or focus it to pause. Reduced-motion settings disable the animation. There is no external feed or server.

## Deploy
Upload the contents of this ZIP to the root of `joethymow/TacoBellMedia`. GitHub Pages → GitHub Actions → Jekyll. `_config.yml` is configured for `/TacoBellMedia`.

To change the design, edit `assets/css/style.css`. `_includes/site.css` is an identical fallback copy used inline if external styles fail. Keep both in sync.

Before replacing your repository, back up any existing articles in `_posts/` and any custom images.
