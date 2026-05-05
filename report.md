# Leaderboard Clone — Report

## Approach

The task was to replicate the internal company leaderboard UI faithfully, without using any real corporate data.

## Tools & Techniques

- **Pure HTML/CSS/JS** — no frameworks or build tools required; the entire app is a single `index.html` file, which makes deployment to GitHub Pages trivial.
- **CSS custom properties** — all colours and radii are defined as CSS variables so the theme is consistent and easy to adjust.
- **Vanilla JS** — filtering (year, quarter, category, free-text search), sorting (click column headers), and row expansion are all handled with plain JavaScript and DOM manipulation. No dependencies.
- **Google Fonts (DM Sans + DM Mono)** — loaded via CDN for clean typography that matches the original's style.

## Data Replacement

The original leaderboard contained real employee names, photos, job titles, and department names. All of it was replaced as follows:

| Original data | Replacement |
|---|---|
| Real names | Fictional names (e.g. *Alice Mercer*, *Bruno Castillo*) |
| Profile photos | Coloured avatar circles showing initials |
| Job titles | Generic but realistic fictional titles |
| Department names | Generic fictional department names |
| Scores & activity counts | Plausible random numbers |

No real corporate data was fed into any AI tool. Fictional values were chosen manually to feel realistic without referencing any real person or organisational structure.

## Structure

```
leaderboard/
├── index.html   # complete application (HTML + CSS + JS)
└── report.md    # this file
```

## Deployment

The app is deployed to **GitHub Pages** directly from the `main` branch root. Steps:

1. Create a new public GitHub repository.
2. Push `index.html` and `report.md` to the `main` branch.
3. Go to *Settings → Pages*, set source to `main` / `root`.
4. GitHub Pages publishes the site automatically at `https://<username>.github.io/<repo>/`.
