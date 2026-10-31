## Version 3 — crest placement refinement

Removed the H badge from the homepage hero and footer. Retained the homepage divider. Added a restrained official H badge to the page introduction on Food Menu, Our Story, Drinks, and Banquets & Events. No other content or functionality changed.

# Hilltop Restaurant Website — V1

Astro static site prepared for GitHub and Cloudflare Workers deployment. **Not deployed.**

## Local preview
1. Install Node.js 20+ if needed.
2. Open a terminal in this folder.
3. Run `npm install` then `npm run dev`. Open the URL shown.
4. Run `npm run build` before uploading. Output is in `dist/`.

## GitHub / Cloudflare
Upload the entire source folder (excluding node_modules and dist) to a new GitHub repository. Cloudflare Workers static asset hosting can build with `npm run build` and serve `dist/` (configure Workers assets in the Cloudflare dashboard). Do not connect or deploy until approved.

## Required before public launch
- **ORDER LINK:** `src/data/site.js` → `orderUrl` is intentionally blank. The visible Order Online button currently goes to Contact and says Soon. Replace its destination in `src/layouts/Layout.astro` with the verified Hilltop SpotOn link. Never use Ellington Pizza's link.
- **EVENT INQUIRIES:** Current form opens a prefilled email in the visitor's email app; it is NOT a server-submitted form. Connect a secure form service/endpoint and test before claiming web submission.
- **PHOTOGRAPHY:** Replace branded placeholder panels with professional Hilltop images after the shoot; do not use generic stock as actual restaurant photography.
- **DRINKS:** Await finalized drinks menu and prices.
- **CONTACT:** Verify public restaurant phone and operating hours; the banquet packet provides 860-477-1054 and hilltopbanquets@gmail.com for event inquiries.
- **BANQUET CAPACITY:** The food menu says 95, buffet/breakfast packet says 90, plated says 85. Package-specific limits are displayed rather than claiming a single universal capacity. Confirm actual occupancy.
- **MENUS:** Compare website menu data with latest approved prices before launch. The PDF files are included unchanged.

## Source organization
- `src/pages/` pages
- `src/layouts/Layout.astro` global header/footer/styles
- `src/data/menu.js` menu items/prices
- `src/data/banquets.js` event packages
- `src/data/site.js` site settings / TODOs
- `public/assets/` official Hilltop logo assets
- `public/menus/` supplied PDFs

## Change log
V1 — initial branded responsive Astro site, categorized food menu, event packages and email inquiry, drinks placeholder, About, Contact, official logos, SEO basics.


## V2 — Crest accents and logo correction
- Official H badge above homepage hero headline, decorative divider after food section, and footer signature.
- Replaced three malformed logo SVGs with corrected versions from the V1 logo fix.
- Added `wrangler.jsonc` for the separate `hilltopwebsite` Cloudflare Worker.
- **Pending:** SpotOn ordering URL, photography, drinks content, and verification of business contact details.
- Upload the **contents** of this folder to the existing `ktena23/HilltopWebsite` GitHub repository, not Ellington Pizza. Cloudflare may automatically deploy commits.
