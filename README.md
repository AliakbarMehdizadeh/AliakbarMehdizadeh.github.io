# aliakbarmehdizadeh.github.io

Personal academic website of Aliakbar (Ali) Mehdizadeh, computational social scientist.

Live at https://aliakbarmehdizadeh.github.io/

## How it is built

A single static page with no build step, served by GitHub Pages from the root of the `main` branch.

| File | What it does |
| --- | --- |
| `index.html` | The whole site: content, styles, search metadata (JSON-LD), and the Fig. 1 network animation |
| `404.html` | Page shown for broken links |
| `robots.txt`, `sitemap.xml` | Tell search engines what to crawl |
| `assets/og-image.png` | Preview image shown when the link is shared |
| `assets/favicon.svg`, `favicon.ico`, `assets/apple-touch-icon.png` | Browser and phone icons |
| `assets/fonts/` | Newsreader typeface (SIL Open Font License, see `OFL.txt`) |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

## Common edits

- **New paper or talk:** copy an existing `<li>` in the Publications or Talks section of `index.html` and edit it. If it is a paper, also add a `ScholarlyArticle` entry to the JSON-LD block in the `<head>`.
- **Add a CV:** put `cv.pdf` in the repository root and add `<li><a href="/cv.pdf">CV</a></li>` to the list of links under the name.
- **Add a photo:** put a square `photo.jpg` in `assets/`, then add `"image": "https://aliakbarmehdizadeh.github.io/assets/photo.jpg"` to the `Person` entry in the JSON-LD block.
- **After any edit:** update the date in `sitemap.xml` (`<lastmod>`), in the JSON-LD (`dateModified`), and in the footer.
