# EZjobhop Website Toolkit

This is a simple static website package for **EZjobhop.com**. It is designed to run for free on GitHub Pages without a build system.

## What is included

- `index.html` — full one-page website with responsive styling and SEO/social metadata
- `404.html` — simple custom error page
- `assets/logo-full.png` — transparent full EZjobhop logo
- `assets/logo-mark.png` — transparent mark used in the header and favicon
- `assets/favicon.ico`, `favicon-32x32.png`, `favicon-16x16.png` — browser tab icons
- `assets/apple-touch-icon.png` — iPhone/iPad home screen icon
- `assets/og-image.png` — LinkedIn/Facebook/iMessage/WhatsApp sharing image, 1200 x 630
- `assets/social-square.png` — square social image, 1200 x 1200
- `site.webmanifest` — app icon metadata
- `robots.txt` and `sitemap.xml` — basic search engine files
- `CNAME` — custom domain file for GitHub Pages
- `.nojekyll` — prevents GitHub Pages from treating the site as a Jekyll project

## Quick GitHub Pages setup

1. Create a new GitHub repository, for example: `ezjobhop-website`.
2. Upload every file and folder from this package to the root of the repository.
3. Go to **Repository → Settings → Pages**.
4. Under **Build and deployment**, choose:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`
5. Under **Custom domain**, enter: `ezjobhop.com`.
6. Turn on **Enforce HTTPS** once GitHub finishes provisioning the certificate.

## GoDaddy DNS setup for GitHub Pages

In GoDaddy DNS management, add/update these records:

| Type | Name | Value |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | YOUR-GITHUB-USERNAME.github.io |

Replace `YOUR-GITHUB-USERNAME` with your actual GitHub username or organization name.

DNS can take time to propagate. GitHub notes that DNS changes may take up to 24 hours.

## Important edits before publishing

Open `index.html` and confirm these details:

- Email: `datawizetechllc@gmail.com`
- Phone: `(513) 926-6663`
- Address: `519 Seneca Green Way, Great Falls, VA 22066, USA`
- Page title and meta description
- Any service language you want to soften, expand, or remove

## Static form note

The contact form currently uses `mailto:` so it opens the visitor's email app. That works for a very simple free site, but it is not as professional as a real form endpoint.

Later, you can connect the form to Formspree, Basin, Netlify Forms, HubSpot, Zoho, or another CRM form endpoint.
