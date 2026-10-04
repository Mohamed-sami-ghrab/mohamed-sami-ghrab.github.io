# Mohamed Sami Ghrab - Portfolio

This is my personal portfolio website and online CV. It is a small static site hosted with GitHub Pages.

The site is available at [mohamed-sami-ghrab.github.io](https://mohamed-sami-ghrab.github.io).

## Updating the site

The page content and styles are in `index.html`. Images and CV files live in `assets/`.

To update the profile photo, replace `assets/img/profile.jpg` with a square image using the same filename. If there is no photo, the page falls back to my initials.

To update the CV, replace `assets/cv/Mohamed_Sami_Ghrab_CV.pdf` and regenerate the preview image:

```bash
pdftoppm -png -r 110 -singlefile assets/cv/Mohamed_Sami_Ghrab_CV.pdf assets/img/cv-preview
```

The current CV date is shown in the CV section of `index.html`.

## Files

```
index.html                 page markup and styles
assets/cv/                  downloadable CV
assets/img/profile.jpg     profile photo
assets/img/cv-preview.png  CV preview for mobile browsers
.nojekyll                  keeps the site fully static on GitHub Pages
```
