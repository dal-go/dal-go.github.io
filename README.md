# dal-go.github.io

Source for **https://dal-go.github.io** — the landing page for the
[DALgo](https://github.com/dal-go/dalgo) ecosystem.

## Stack

Plain static HTML + CSS. No build step. GitHub Pages serves the contents of
`main` directly (a `.nojekyll` file disables Jekyll processing).

## Local preview

```sh
# any static server works
python3 -m http.server 8000
# then open http://localhost:8000
```

## Editing

- `index.html` — page content and structure.
- `styles.css` — design system: fonts, colors, layout, motion.
- `.nojekyll` — keep this file; it tells GitHub Pages to serve files as-is.

When adding a new adapter to the DALgo org, also add a card to the **Adapters**
section in `index.html`.

## License

MIT — see `LICENSE`.
