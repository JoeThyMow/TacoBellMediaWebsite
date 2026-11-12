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


## Typography and ticker
This edition uses Times New Roman throughout and a fast, right-moving newswire (9-second loop). CSS is duplicated in `_includes/site.css` as a GitHub Pages fallback. Update both stylesheets when editing the theme.


## Classic edition
This version uses Times New Roman, flat purple navigation, compact newspaper typography, and a fast right-moving newswire. To publish, add a dated Markdown post to `_posts/`.

## Ad images and lead news photograph
- Upload your left ad as `assets/images/ads/left-ad.png`.
- Upload your right ad as `assets/images/ads/right-ad.png`.
- Both side ads appear on sufficiently wide desktop screens (they are hidden on narrower screens).
- Ads currently link to `#`. Change the `<a href="#">` in `_layouts/default.html` if an advertiser supplies a destination.
- Upload a news photo to `assets/images/news/election-results.jpg`, then uncomment the `image:` line in `_posts/2026-11-12-election-results.md`.
- The homepage displays the newest article photo, followed by `LATEST NEWS:` and its title.

## Layout repair
The header logo is included at `assets/images/taco-bell-logo.png` and constrained to 76 × 76 pixels. Ads stay outside the 940px centered website and are hidden on narrow screens. If the page is still unstyled, check that `_config.yml` has `baseurl: "/TacoBellMedia"` and upload the *contents* of this ZIP to the repository root.
