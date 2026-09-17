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
- **About** — bio paragraphs, quick facts
- **Skills** — tag pills grouped by category
- **Work** — project cards; each `.work-card__media` div holds an `<img>` pointing at a file
  in `assets/`, sized/cropped to the card's 16:10 aspect so nothing gets clipped by CSS
- **Experience** — timeline entries
- **Contact** — email address and social links (repeated in the hero and contact section)

Social links (Instagram/LinkedIn/X) and the contact email are already filled in.

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
