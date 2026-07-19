# Price Truth Website

Static marketing, privacy, terms, and support website for Price Truth.

## Website files

- `index.html` — marketing page
- `privacy.html` — privacy policy
- `terms.html` — terms of service
- `support.html` — customer support
- `styles.css` and `script.js` — shared presentation and navigation behavior
- `assets/` — Price Truth icon and product media

## Hosting with IONOS

This is a static website and does not require a database, Node.js, or a build command.

When connecting the repository to IONOS:

- Repository: `Optiva-RS/pricetruth-website`
- Branch: `main`
- Build command: leave blank
- Publish or output directory: `/` (repository root)
- Entry file: `index.html`

Connect `price-truth.com` only after the IONOS preview URL has been verified. The public website intentionally does not link to the authenticated Base44 application URL.

## Safe cutover order

1. Push this repository and create the IONOS deployment.
2. Verify the IONOS preview on desktop and mobile.
3. Disconnect `price-truth.com` from the Base44 app.
4. Point the domain to the IONOS deployment using the DNS records IONOS supplies.
5. Confirm HTTPS and all four public pages.

The Base44 application remains the backend for the native iOS app and continues using app ID `6984e9932ccbaa826b4acd4a`.
