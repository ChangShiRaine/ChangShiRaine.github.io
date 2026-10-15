Source for Chang Shi's academic website: https://changshiraine.github.io/

Static pages (`index.html` for About/Research, `projects.html` for Projects, shared `stylesheet.css`), adapted from [Jon Barron's website template](https://github.com/jonbarron/jonbarron.github.io). `.nojekyll` tells GitHub Pages to serve the files as-is.

- Paper and project thumbnails live in `images/papers/` and `images/` (about 160px wide when displayed).
- PDFs (CV, reports, posters) live in `files/`.
- To add a paper, copy one `<tr>...</tr>` block in the Research table of `index.html`; projects work the same way in `projects.html`.
- The top nav tabs are duplicated in every page (the `<header class="site-header">` block); edit all of them when adding a tab.
