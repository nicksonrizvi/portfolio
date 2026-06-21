# najmaz.sakib — Personal Portfolio

Personal portfolio website for **Najmaz Sakib** — Senior Engineer, Service Assurance at Infozillion Teletech BD Ltd. Also a singer-songwriter (Nickson Rizvi) and occasional writer.

Live structure: centered single-column layout, light/dark mode toggle, fully responsive (desktop, laptop, tablet, mobile).

## Files

```
index.html   — Home page (About, Now, Music, Writing, Find, Contact)
cv.html      — Full CV / résumé
style.css    — Shared stylesheet (typography, theme, layout)
photo.jpg    — Profile photo (used on CV page)
README.md    — This file
```

## Design system

- **Fonts:** DM Sans (body), DM Mono (labels/dates), Instrument Serif (name/headings)
- **Light mode:** warm off-white background, soft charcoal text
- **Dark mode:** Claude.ai-inspired warm charcoal palette with terracotta accent
- **Layout:** centered single column, max-width 620px, no sidebar
- Dark/light preference saved in the visitor's browser (`localStorage`)

## Updating content

- **Bio / sections** → edit directly inside `index.html` (`<section class="section">` blocks)
- **CV entries** → edit inside `cv.html` (`<div class="cv-section">` blocks)
- **Colors / fonts / spacing** → edit CSS variables at the top of `style.css` (`:root` and `[data-theme="dark"]`)
- **"Last updated" badge** → plain text in the footer of `index.html`; update the month/year manually when you make changes

## Deploy on GitHub Pages

1. Push all files to your GitHub Pages repository (e.g. `sakib-opsgrid/portfolio` or `<username>.github.io`)
2. Go to **Settings → Pages**
3. Under **Source**, select **Deploy from a branch**
4. Choose the **main** branch, **/ (root)** folder → **Save**
5. Site goes live at your GitHub Pages URL within a minute or two

## Notes

- No build step, no dependencies — plain HTML/CSS/JS, works anywhere static files are served
- Fonts loaded from Google Fonts via `<link rel="preconnect">` + CSS `@import`
- Fully keyboard- and screen-reader-friendly semantic HTML
