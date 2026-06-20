# kushantp58.github.io

Personal portfolio for **Kushant Patel** — robotics, perception, and control engineer.
A single static page, no build step, no framework: HTML, CSS, and a little vanilla JS.

## Structure

```
docs/
├── index.html              # the whole site
├── 404.html                # themed not-found page
├── .nojekyll               # serve files as-is (skip Jekyll)
├── README.md
└── assets/img/
    ├── favicon.svg · favicon-180.png
    ├── og.svg · og.png             # social share card (1200x630)
    └── photos/                     # profile + "In the Field" gallery
        ├── portrait.jpg
        ├── field-brookhaven.jpg · field-spot-team.jpg
        ├── field-watonomous-team.jpg · field-av.jpg
        └── field-ucdavis.jpg · field-waterloo.jpg
```

## Deploy

Pages already builds from **/docs on the gh-pages branch**, so:

1. Replace the contents of `docs/` on `gh-pages` with this `docs/` folder.
2. Commit and push. No other Settings change needed.
3. The `.nojekyll` file stops GitHub from running the old Jekyll theme over these files.
   You can delete the now-unused `_config.yml`, `_layouts`, `_includes`, `_sass`,
   `_data`, `_works`, `Gemfile*`, `about.md`, and `search.json`.

Live at: https://kushantp58.github.io

## Personalize later

- Resume link -> two links (top nav + contact) point to your Google Drive CV; swap the URL
  or host the PDF in `docs/assets/` and point to it.
- Blog posts -> both essay cards link to your Medium profile; replace with direct post URLs.
- Photos -> all in `assets/img/photos/`. Drop in replacements with the same filename,
  or edit the `<img src>` paths in `index.html`. EXIF/GPS was stripped on export.

## Notes

- Respects `prefers-reduced-motion` (the LiDAR hero freezes to a static point cloud).
- Responsive to mobile; keyboard focus styles included; no external JS dependencies.
