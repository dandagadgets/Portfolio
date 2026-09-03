# Portfolio

A clean, modern, single-page portfolio site. No build step — plain HTML/CSS/JS.

## Structure

```
index.html      All page content and sections
css/style.css   Styling, theme (light/dark), layout
js/main.js      Theme toggle, mobile nav, scroll reveal, contact form
```

## Customize

Everything you need to change lives in `index.html`:

- **Title/meta** — `<title>` and `<meta name="description">` in `<head>`
- **Hero** — your name, tagline, rotating words (also edit the `words` array in `js/main.js`)
- **About** — bio paragraphs, quick facts, résumé link (`resume.pdf`, add the file yourself)
- **Skills** — tag pills grouped by category
- **Work** — project cards; replace the numbered gradient placeholders with real screenshots by
  swapping the `.work-card__media` div for an `<img>`, and update the live/code links
- **Experience** — timeline entries
- **Contact** — email address and social links (repeated in the hero and contact section)

Social links (GitHub/LinkedIn/X) and the contact email currently point to placeholder
addresses (`yourhandle`, `you@example.com`) — search and replace them.

The contact form doesn't submit anywhere yet. Point its `action` at a form service like
[Formspree](https://formspree.io) or [Getform](https://getform.io), or swap the JS handler in
`js/main.js` for a `fetch()` call to your own backend.

## Run locally

No build tools needed — just open `index.html` in a browser, or serve the folder:

```
python3 -m http.server 8000
```

## Deploy (GitHub Pages)

1. Push this repo to GitHub (already done if you're reading this from there).
2. Repo **Settings → Pages → Source**: select the `main` branch, `/ (root)` folder.
3. Your site will be live at `https://<username>.github.io/<repo>/`.
