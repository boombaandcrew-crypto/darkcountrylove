# Dark Country Love Landing Page

Modern artist landing page for Dark Country Love — a clean, dark, editorial-style static site ready for Vercel.

## Design notes

- Contemporary typography (Instrument Serif + Inter)
- Minimal chrome, strong hierarchy, refined gold accents
- Sticky glass header, mobile menu, scroll reveals
- Same streaming + social links and image asset paths as before
- Vercel Web Analytics support after deployment

## Local Preview

Open `index.html` directly in a browser, or run a tiny local server:

```bash
npx serve .
```

Place the `assets/` folder next to `index.html` (same structure as the original project).

## Production Deploy With Vercel

1. Create a new GitHub repository for this folder.
2. Push the contents (including `assets/`) to that repository.
3. In Vercel, choose **Add New Project** and import the GitHub repository.
4. Keep the default static-site settings. No build command is required.
5. Deploy and test the generated Vercel URL.
6. In the Vercel project dashboard, enable **Web Analytics**.
7. Visit the production site and wait for page views to appear in Vercel Analytics.

## Visitor Analytics

This static site includes Vercel Web Analytics via `/_vercel/insights/script.js`.
It will not collect visits from `localhost`; it starts collecting after the site is deployed on Vercel and Web Analytics is enabled for the project.

## Custom Domain With Cloudflare

1. In Cloudflare Registrar, search for `darkcountrylove.com`.
2. Buy it if available, or choose a close alternative.
3. In Vercel, open the project and add these domains:
   - `darkcountrylove.com`
   - `www.darkcountrylove.com`
4. In Cloudflare DNS, use these Vercel records:
   - `A` record for `@` -> `76.76.21.21`
   - `CNAME` record for `www` -> `cname.vercel-dns.com`
5. Remove old/conflicting `A` records for `@` or `www`, especially records pointing to non-Vercel IPs.
6. Wait for Vercel to show HTTPS as active.
7. Test both final URLs:
   - `https://darkcountrylove.com`
   - `https://www.darkcountrylove.com`

## Redeploy Note

Updated deployment docs for the custom domain DNS records. Push this README change to trigger a fresh Vercel deployment after DNS is corrected.

## Current Streaming Links

- Spotify: https://open.spotify.com/artist/5lqI0gSjYDzpQOC0ykbICW?si=wf2gkW0vRR6AXW1o1JJegw
- YouTube Music: https://music.youtube.com/@darkcountryloveofficial?si=BKmzCbQlw4bOp9Lq
- Apple Music: https://music.apple.com/us/album/carry-me-when-i-cant-stand-single/6792970401

## Current Social Links

- Facebook: https://www.facebook.com/profile.php?id=100078061854185
- Instagram: https://www.instagram.com/dark.country.love/
- TikTok: https://www.tiktok.com/@dark.country.love
