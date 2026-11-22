# aliakbarmehdizadeh.github.io

Personal academic website of Aliakbar (Ali) Mehdizadeh, complex systems researcher.

Live at https://aliakbarmehdizadeh.github.io/

## How it is built

A single static page with no build step, served by GitHub Pages from the root of the `main` branch.

| File | What it does |
| --- | --- |
| `index.html` | The whole site: content, styles, search metadata (JSON-LD), and the Fig. 1 network animation |
| `404.html` | Page shown for broken links |
| `Mehdizadeh_CV.pdf` | CV linked from the page |
| `robots.txt`, `sitemap.xml` | Tell search engines what to crawl |
| `assets/og-image.png` | Preview image shown when the link is shared |
| `assets/favicon.svg`, `favicon.ico`, `assets/apple-touch-icon.png` | Browser and phone icons |
| `assets/fonts/` | Newsreader typeface (SIL Open Font License, see `OFL.txt`) |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

## Common edits

- **New paper or talk:** copy an existing `<li>` in the Publications or Talks section of `index.html` and edit it. If it is a paper, also add a `ScholarlyArticle` entry to the JSON-LD block in the `<head>`.
- **Update the CV:** replace `Mehdizadeh_CV.pdf` with a new PDF of the same name. Its LaTeX source is `CV_Mehdizadeh_Website.tex` in the CV_Letter folder; this public copy leaves out the phone number.
- **Change the photo:** replace `assets/photo.jpg` with another square image (at least 440 pixels, metadata removed). The page and the JSON-LD `Person` entry both point to it.
- **After any edit:** update the date in `sitemap.xml` (`<lastmod>`), in the JSON-LD (`dateModified`), and in the footer.
