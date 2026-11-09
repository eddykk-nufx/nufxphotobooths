# NUFXphotobooths — Website (v1)

Live site: https://nufxphotobooths.com  (hosted on Vercel, auto-deploys from GitHub)

Dark theme, cyan accent, real media, all 8 client logos, favicon, cycling showreel hero,
four booth types, Book-Now pricing panel, Web3Forms booking, and GA4 analytics.

## Deploy an update
Re-upload these files to the GitHub repo (Add file > Upload files > drag in > Commit).
Vercel redeploys automatically in ~30-60s.

## Integrations baked in
- Booking form: posts to Web3Forms -> emails Nufx360activations@gmail.com
  (access key is in index.html at `var WEB3FORMS_KEY`).
- Analytics: Google Analytics 4, Measurement ID G-ESXXDSXDXY, loaded in <head>.
- Pricing panel: edit tiers inside <div id="pricingModal"> in index.html.

## Structure
    index.html                 homepage (GA4 tag in <head>)
    favicon.ico                browser tab icon
    assets/img/svc_*.webp      booth cover photos
    assets/img/*.webp          gallery photos + poster frames
    assets/video/reel*.mp4     hero showreels, pillarboxed (cycle 1,2,6,10,5,11,13)
    assets/video/hero.mp4      full showreel ("Watch the showreel" modal)
    assets/video/bmagazine.mp4 magazine booth clip
    assets/logos/*.png         all 8 client logos

## Notes
- Address matches the Google Business Profile exactly (NAP consistency).
- Respects prefers-reduced-motion. Fonts: Poppins + Roboto via Google Fonts.
