# Taco Bell Media — repaired GitHub Pages site

Upload **the contents** of this ZIP to the root of `joethymow/TacoBellMedia`.

This version has ONE shared page layout (`_layouts/default.html`) and a small homepage (`index.html`). The header, logo, news ticker, and ad columns are in the shared layout. Do not upload the enclosing folder.

## Publishing

Add a Markdown article to `_posts/` using `YYYY-MM-DD-title.md`. The newest post becomes the lead story and appears under **LATEST NEWS:**. `Election results` is included as temporary placeholder coverage.

## Photos and ads

- Left ad: `assets/images/ads/left-ad.png`
- Right ad: `assets/images/ads/right-ad.png`
- Lead story photo: upload `assets/images/news/election-results.jpg` and uncomment `image: /assets/images/news/election-results.jpg` in the election post.
- Side ad placeholders are visible on desktop screens wider than 1550px; on smaller screens they hide to protect readability.

## GitHub Pages

In Settings → Pages, use GitHub Actions → Jekyll. The `_config.yml` already uses `baseurl: /TacoBellMedia`. Wait for the Actions workflow to succeed and hard-refresh the browser.
