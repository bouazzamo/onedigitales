# OneDigitales Official Website

Static website for **onedigitales.com** designed for GitHub Pages.

## Pages and Files

- `index.html` - Home page (agency style + app cards)
- `app-privacy-policy/index.html` - Privacy policy page (clean URL: `/app-privacy-policy/`)
- `app-ads.txt` - AdMob app-ads declaration file
- `CNAME` - Custom domain mapping (`onedigitales.com`)
- `.nojekyll` - Disables Jekyll processing on GitHub Pages
- `assets/images/Logo.png` - Official OneDigitales logo
- `assets/images/Favicon.png` - Site favicon

## Publish to GitHub Pages

1. Push this folder to a GitHub repository (for example: `onedigitalesdev`).
2. On GitHub: **Settings > Pages**.
3. Under **Build and deployment**, set:
   - Source: `Deploy from a branch`
   - Branch: `main` (or your active branch), folder `/ (root)`
4. Save and wait for deployment.

## Connect Custom Domain

1. Confirm `CNAME` contains only:
   - `onedigitales.com`
2. In your domain DNS provider, add:
   - `A` record for `@` pointing to GitHub Pages IPs
   - `CNAME` record for `www` pointing to `<your-github-username>.github.io`
3. In GitHub Pages settings, ensure **Custom domain** is `onedigitales.com`.
4. Enable **Enforce HTTPS** after DNS propagation.

## AdMob Note

Replace the placeholder publisher ID in `app-ads.txt`:

- Current: `pub-0000000000000000`
- Replace with your real AdMob publisher ID.
