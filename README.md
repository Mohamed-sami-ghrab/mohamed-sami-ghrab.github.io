# Mohamed Sami Ghrab · Portfolio

Personal portfolio and CV, published with GitHub Pages.

## Publish on GitHub Pages

1. On GitHub, create a new **public** repository named exactly `mohamed-sami-ghrab.github.io`.
2. Upload everything in this folder (keep the folder structure: `index.html`, `assets/`, `.nojekyll`).
3. Go to **Settings → Pages**, set **Source** to *Deploy from a branch*, branch `main`, folder `/ (root)`, and save.
4. After a minute or two the site is live at **https://mohamed-sami-ghrab.github.io**.

## Change the photo

Replace `assets/img/profile.jpg` with your picture (square, at least 400×400 px, same file name). If the file is missing, the page shows your initials instead.

## Update the CV

Replace `assets/cv/Mohamed_Sami_Ghrab_CV.pdf` with the new PDF (same file name), then regenerate the preview image used on phones:

```bash
pdftoppm -png -r 110 -singlefile assets/cv/Mohamed_Sami_Ghrab_CV.pdf assets/img/cv-preview
```

Update the "Updated October 2026" line in the CV section of `index.html`.

## Structure

```
index.html                     the whole site (HTML + CSS, no build step)
assets/cv/…CV.pdf              downloadable / embedded CV
assets/img/profile.jpg         portrait
assets/img/cv-preview.png      CV preview for mobile browsers
.nojekyll                      serve files as-is on GitHub Pages
```
