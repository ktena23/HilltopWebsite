# Hilltop Restaurant Website — V7

Complete Astro static website for Hilltop Restaurant. Built from the V4 baseline, with carefully integrated V5 content changes.

## Changes
- Removed announcement strip.
- Homepage retains Warm White header and standard logo.
- Interior pages have Espresso header, cream navigation and ordering placeholder, and official reversed logo.
- Our Story moved after Contact in desktop and mobile navigation.
- Contact page includes Ellington Pizza and Beni's logos, addresses and phone numbers, Hilltop hours, and note on extended bar hours.
- Food Menu hero title reduced and vertical spacing tightened.
- Latest food menu PDF and banquet PDF retained.

## Deploy
Upload the **contents** of this folder to the root of the existing `ktena23/HilltopWebsite` GitHub repository (do not upload the ZIP itself). Commit to main; Cloudflare Git integration should redeploy.

## Configuration
Cloudflare Worker name: `hilltopwebsite`; build command `npm run build`; deploy command `npx wrangler deploy`. Wrangler config serves `./dist`.

## Pending
- Add correct Hilltop SpotOn ordering URL in `src/data/site.js` and wire button after approval.
- Professional restaurant photography.
- Drinks content.
- Banquet form backend (currently mailto-based).

## Verification
Source and ZIP integrity checked. Production Astro build could not be completed in this environment because npm dependency installation timed out. Check Cloudflare build logs before treating V7 as validated.
