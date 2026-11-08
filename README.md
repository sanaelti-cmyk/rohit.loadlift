# LoadLift executive profile

Self-contained static website. No build step, external font requests, API keys, backend or runtime dependencies. Fonts and original SVG branding are copied locally from the supplied main website source. Open index.html or serve this folder with any static server.

## Editorial and artwork review
Introductions, contributions and responsibilities are role-based drafts supplied for review; they are not verified achievements. Review before publishing. No founder status, employment history, awards or metrics are claimed. The B.Tech in Computer Science and Engineering at KIIT, Bhubaneswar, India, was confirmed by the user for all three team members; graduation dates and additional qualifications are not stated. Team-supplied portraits are included locally and matched using the supplied filenames. Original photo files are preserved; display cropping uses CSS only. Update the marked HTML comments to replace introduction/contribution text or the authorized portrait.

Only an Aniket business-card screenshot was supplied. The legacy logo.png and card-front.png are proportion-preserving crops of that reference. The visible header, footer and card use the original loadlift-icon-mark.svg from the supplied main website source. Aniket's card-back.png is a crop of the supplied card. Ritesh and Rohit's card-back.png files are newly typeset matching artwork using the supplied details, not claimed to be original cards. Replace with approved original artwork when available. The full supplied reference is retained in assets/branding-reference.png. Social sharing uses a locally generated 1200×630 image.

## Upload and GitHub Pages setup (manual)
Upload the CONTENTS of this folder (including assets, index.html, CNAME, .nojekyll and the .vcf file) into the root of its matching repository. Do not upload the parent folder as an extra directory. Existing Git clones can commit and push these files normally.

In repository Settings → Pages, select Deploy from a branch, choose the main branch and / (root), then Save. Add the profile subdomain below as the Custom domain and save. The included CNAME contains exactly that domain. These steps are instructions only; Pages and DNS have not been enabled automatically.

Custom domain: `rohit.loadlift.com.np`

At the DNS provider for loadlift.com.np, create:

| Type | Host | Target |
| --- | --- | --- |
| CNAME | ritesh | YOUR_GITHUB_USERNAME.github.io |
| CNAME | aniket | YOUR_GITHUB_USERNAME.github.io |
| CNAME | rohit | YOUR_GITHUB_USERNAME.github.io |

YOUR_GITHUB_USERNAME is an explicit placeholder: replace it with the GitHub user or organization that OWNS these repositories (for the supplied URLs, sanaelti-cmyk). Do not include a repository path, https://, or the profile domain in the target. Configure each subdomain in its corresponding repository. Avoid conflicting records or wildcard records. Verify domain ownership in GitHub if applicable.

Wait for DNS validation and certificate provisioning, then select Enforce HTTPS in Settings → Pages. GitHub notes this option can take up to 24 hours to become available. QR destinations become accessible only after deployment, DNS configuration and HTTPS activation. The QR files encode the direct custom-domain URL; they do not use tracking or redirects. Before printing cards, scan the final printed proof and check the live HTTPS page on a phone.

Official GitHub documentation checked 2026-11-08:
- https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/securing-your-github-pages-site-with-https

## Files and updates
- index.html contains all CSS and minimal vanilla JavaScript for the mobile menu, English/Nepali text switch and light/dark theme. Content and links also work without JavaScript; on phones the menu requires JavaScript.
- contact.vcf is a UTF-8 vCard 3.0 contact with phone, email, role, company and profile URL.
- assets/profile-qr.svg is a printing-friendly QR; assets/profile-qr.png is a high-resolution PNG. Both have black modules, white background and a four-module quiet zone with no overlay.
- assets/social.png, favicon.png, logo.png and both card images are local assets.
- When changing a profile URL, regenerate BOTH QR formats with a QR encoding library and independently decode both. Update canonical/social metadata, CNAME and contact.vcf together.

## Main website header, footer and revised contact card
The supplied React source (landing.tsx and LoadingSequence.tsx / HalftoneWordmarkFooter) was adapted to standalone HTML, inline CSS and minimal vanilla JavaScript. No React runtime is used. The source logo, local fonts, footer content, LinkedIn URL and Nepal map are retained. The footer wordmark uses a static dotted SVG instead of a canvas animation. Main-site links use absolute HTTPS URLs: /home, /home#loadlift-milestones, /home#container-loading, /track, /login and /login#signup. Contact scrolls to this page's matching company footer. Company contact@ email is also retained. Source footer office, support and fee copy is copied as supplied and should be reviewed by the company.

The People and Stay Connected sections were removed at the user's request. The Let's Connect section now has an HTML business card: genuine QR on the left; name, role, clickable phone and email on the right. QR download links and profile URL sit directly below. Previous card artwork remains in a collapsed disclosure.
