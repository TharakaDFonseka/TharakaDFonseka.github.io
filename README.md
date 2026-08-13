# Personal Academic Website — Tharaka D. Fonseka

A single-page, dependency-free academic website (plain HTML/CSS/JS) ready for GitHub Pages.

## Structure

```
tharaka-website/
├── index.html          # All content lives here
├── css/style.css       # Theme (colors, layout, responsive rules)
├── js/main.js          # Nav highlighting, mobile menu, scroll reveal
└── assets/
    └── profile-placeholder.svg   # Replace with your photo
```

## Before publishing — TODO checklist

1. **Photo**: add your photo as `assets/profile.jpg` and change the `<img src=...>`
   in the hero section of `index.html` from `assets/profile-placeholder.svg` to `assets/profile.jpg`.
2. **CV**: add your CV PDF as `assets/cv.pdf` (two links point to it: hero and contact).
3. **Google Scholar / GitHub links**: search `index.html` for `href="#"` (marked with
   `TODO` comments) and replace with your real profile URLs. There are two of each
   (one in the hero, one in the contact section).
4. Review the content (dates, wording) — everything was compiled from your Canva site,
   LinkedIn, and public paper listings.

## Deploying to GitHub Pages

The site lives in the `TharakaDFonseka/TharakaDFonseka.github.io` repository.
To publish changes:

```bash
git add .
git commit -m "Update website"
git push
```

If Pages isn't enabled yet, go to **Settings → Pages → Source: Deploy from a branch → main / (root)**.
The site is served at `https://tharakadfonseka.github.io`.

## Previewing locally

Open `index.html` directly in a browser, or run a tiny server:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Customizing

- **Accent color**: edit `--accent` (and `--accent-dark`, `--accent-soft`) at the top of
  `css/style.css`. Currently deep green (`#2e7d32`).
- **Adding news items**: copy any `<li>` inside the `news-list` in `index.html`.
- **Adding publications**: copy an `<li>` inside the relevant `pub-list`.
