# Debjoy Thakur Academic Website

This folder is ready for GitHub Pages.

## Upload instructions

1. Open your GitHub repository: `debjoythakur/debjoy.github.io`.
2. Upload **the contents of this ZIP**, not the outer ZIP folder itself.
3. Make sure `index.html` is visible at the top level of the repository.
4. Go to **Settings → Pages**.
5. Under **Build and deployment**, choose:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/ (root)`
6. Save.
7. After deployment, your site should appear at:
   `https://debjoythakur.github.io/`

## Add your photograph

The current homepage shows a circular `DT` placeholder.

To use your photograph:
1. Add your photo to the `assets` folder and call it `debjoy.jpg`.
2. In `index.html`, replace:

```html
<div class="avatar-placeholder">DT</div>
```

with:

```html
<img class="profile-photo" src="assets/debjoy.jpg" alt="Debjoy Thakur">
```

3. Add this CSS to `assets/style.css`:

```css
.profile-photo{
  width:110px;
  height:110px;
  border-radius:50%;
  object-fit:cover;
  margin-bottom:22px;
}
```

## Add your CV PDF

Compile your latest CV in Overleaf and download the PDF.

Rename it:

`Debjoy_Thakur_CV.pdf`

Upload it into:

`files/`

Then add this button to `cv.html` inside the existing button row:

```html
<a class="btn primary" href="files/Debjoy_Thakur_CV.pdf" target="_blank">Download CV PDF</a>
```

## Add research code

Keep code in separate repositories. Recommended examples:

- `localLASSO`
- `gpdpenCNN`
- `vreml-spatial`
- `spatial-intensity-selection`
- `local-lasso-spatial`
- `manifold-pcf`

Then replace the placeholder GitHub links on `software.html` and add `[Code]` links beside the corresponding papers on `publications.html`.

## Main files

- `index.html` — homepage
- `research.html` — research program
- `publications.html` — publications/preprints
- `software.html` — software and code
- `teaching.html` — teaching portfolio
- `cv.html` — CV summary and download
- `assets/style.css` — all visual styling
- `assets/script.js` — mobile navigation and copyright year

No Jekyll, npm, Python, or build step is required.
