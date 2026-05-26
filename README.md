# (moment)

An ambient mobile-first haiku reader. Nine fragments, scrolled slowly.

Live experience: open `moment.html` in a browser, or deploy to any static host.

## Deploy

Drop both files at the root of any static host (Vercel, Netlify, GitHub Pages, S3, …).
URL: `your-host.com/moment.html`. No build step.

```
moment.html
moment.jsx
```

`moment.html` is the entry point. It loads React (production), Babel (in-browser JSX), Manrope + Newsreader + DM Mono from Google Fonts, and `moment.jsx`. No bundler.

## Local

Any static-file server works. Examples:

```bash
python3 -m http.server 8000
# or
npx serve .
```

Then open `http://localhost:8000/moment.html`.

## Interaction

- Scroll vertically through nine fragments.
- A faint horizon line migrates with each fragment.
- The experience silently loops after the final credits.
- `prefers-reduced-motion` is respected — fades shorten, drift is removed.

## Credits

Haikus written and designed by **Pankti Porecha**, May 2026.
