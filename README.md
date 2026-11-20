# Reetika Raj — Portfolio

Personal portfolio of Reetika Raj, M.Des (Product Design, Development & Management), IISc Bengaluru.
Built with [Astro](https://astro.build) as a static site and hosted on Netlify.

## Case studies

| Page | Project |
|---|---|
| `/work/inclusive-cafe-table` | A Table for Everyone: an inclusive, height-adjustable café table |
| `/work/posture-buddy` | Posture Buddy: a desk companion that notices slouching |
| `/work/aasan` | Aasan: an ergonomic classroom chair |
| `/work/crib-collection` | Beneath the Water, Into the Snow: a crib collection and play gym |

## Run it on your computer

You need [Node.js](https://nodejs.org) 18.17 or newer.

```bash
npm install      # first time only
npm run dev      # opens a live preview at http://localhost:4321
```

## Build

```bash
npm run build    # writes the finished site to dist/
npm run preview  # previews the built site
```

## Deploy

The repository is connected to Netlify. Every push to the main branch rebuilds and publishes the site
automatically, using the settings in `netlify.toml` (build command `npm run build`, publish folder `dist`).

## Where things live

```
src/
  pages/          index.astro (home) and work/ (one file per case study)
  components/     reusable pieces: ID card, rolling project cards, diagrams, trees
  layouts/        Base.astro: page shell, navigation, footer
  styles/         global.css (colours, type, motion) and case.css (case-study styles)
public/           files served as-is: images, logos, CV, cursor, favicon
```

- **Change the CV:** replace `public/Reetika_Raj_CV.pdf` (keep the same file name).
- **Change the ID-card photo:** replace `public/reetika.jpg`.
- **Edit a case study:** open its file in `src/pages/work/`.
