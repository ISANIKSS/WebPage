# ISANIK Website (single-page)

## How to run locally
Open `index.html` in a browser (or use VS Code Live Server).

## Make the contact form actually send email (GitHub Pages)
GitHub Pages cannot send email directly from HTML.

**Recommended (works in 5 minutes): Formspree**
1. Create a Formspree form (Free plan is enough).
2. Copy the endpoint URL (looks like `https://formspree.io/f/xxxxxx`).
3. In `index.html`, find:
   `<input type="hidden" id="formEndpoint" value="FORM_ENDPOINT" />`
4. Replace `FORM_ENDPOINT` with your real endpoint URL.

If you don't set this, the page still works and the **Email directly** button opens your mail client.

## Where to add your images
- Hero screenshot:
  - Put a PNG in `assets/hero-dashboard.png`
  - In `index.html`, replace `assets/hero-illustration.svg` with `assets/hero-dashboard.png`
- Deployment diagram:
  - Put in `assets/deployment-diagram.png`
  - Replace the second `hero-illustration.svg` reference.

## Brand assets already included
- `assets/logo-horizontal.svg` (header)
- `assets/logo-stacked.svg` (footer)
- `assets/logo-mark.svg` (icon mark)
- `favicon/` package (includes `site.webmanifest`, Apple touch icon, favicon ico/pngs)

