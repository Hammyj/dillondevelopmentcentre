# Football Coaching Static Site

A simple single-page brochure website for a football coaching business. It is built with plain HTML, CSS, and a tiny amount of JavaScript, so it can be deployed directly to Cloudflare Pages from GitHub.

## Edit These First

- Business name: replace `Your Coaching Name` in `index.html`.
- Logo: replace the text mark in the header, or add your logo to `assets/images/` and update the header markup.
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

## Cloudflare Pages

Recommended Cloudflare Pages settings:

- Framework preset: None
- Build command: leave blank
- Build output directory: `/`

Connect the GitHub repository, push these files, and Cloudflare Pages can serve the site as-is.
