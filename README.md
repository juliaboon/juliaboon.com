# juliaboon.com

Static site. No build step, no framework, no tracking.

- `index.html` — the register
- `style.css` — all styling
- `CNAME` — tells GitHub Pages the custom domain
- `documents/` — PDFs, linked from entries

## Editing

Each filing is one `<li class="entry">` block in `index.html`. Copy an existing
block, change the date, title, description and docket line. Newest at the top.

To publish a held document: replace the `<span class="hold">…</span>` with a link,
e.g. `<a href="documents/manifesto-trs.pdf">PDF · 1.2&nbsp;MB</a>`

## Deploy

Commit to `main`. GitHub Pages rebuilds in about a minute.
