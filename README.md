# Football Coaching Static Site

A simple single-page brochure website for a football coaching business. It is built with plain HTML, CSS, and a tiny amount of JavaScript, so it can be deployed directly to Cloudflare Pages from GitHub.

## Edit These First

- Business name: update `Dillon Development Centre` in `index.html` if the final trading name changes.
- Logo: the current logo is saved at `assets/images/ddc-logo.png`. Replace this file with a higher-resolution version when available.
- Contact details: update phone, email, location, and Instagram handle in the contact section.
- Privacy policy: add `privacy-policy.html` or change the footer link to the final policy URL.
- Photos: replace `assets/images/football-coaching-session.png` with real coaching photos and update the gallery image paths.

## Instagram Feed Options

Pure static HTML cannot automatically pull new Instagram posts without some kind of external service or API token.

Practical options:

- Easiest: link to Instagram and update the gallery manually.
- Low maintenance: use an Instagram feed embed service and paste its script into the gallery section.
- Most controlled: use the Instagram Graph API with a small scheduled build process that writes recent posts into a JSON file before deployment.

For day one, the current gallery keeps the site fast and dependable.

## Future Updates

For a non-technical owner, the best upgrade path is usually a lightweight Git-backed CMS such as Decap CMS, CloudCannon, or TinaCMS. That would let your friend edit events or announcements through a browser while the site still deploys as static files.

## Brand Palette

The current palette is based on the supplied DDC logo, adjusted for readable contrast:

- Charcoal: `#202221` / `#242524`
- Warm cream: `#f2edba`
- Strong cream accent: `#e5d968`
- Pale blue-grey: `#c6d4d6`
- Muted pitch green: `#315542`
- Soft page background: `#f6f3e8`

The cream is used sparingly for accents and buttons, with charcoal used for high-contrast text and panels.

## Cloudflare Pages

Recommended Cloudflare Pages settings:

- Framework preset: None
- Build command: leave blank
- Build output directory: `/`

Connect the GitHub repository, push these files, and Cloudflare Pages can serve the site as-is.
