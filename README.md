# NUFXphotobooths — Website (v1)

Production-ready static homepage: dark theme, cyan accent, real media, all 8 client logos,
favicon, cycling showreel hero, four booth types, and a Book Now pricing & packages panel.

## Run locally
Open index.html, or serve the folder:  npx serve .   (or)   python3 -m http.server

## Deploy (Vercel — free)
1. Push this folder to a repo, or drag it into https://vercel.com/new
2. Preset: "Other" (static, no build step).  3. Add your domain under Settings > Domains.

## Pricing panel
- "Book Now" / "Get pricing" opens a tabbed panel: 360 / Magic Mirror / Magazine / Selfie.
- Each "Book this package" pre-fills the Check Your Date form (booth + package) so the
  enquiry email states exactly what the customer picked.
- To change prices or packages: edit the tiers inside <div id="pricingModal"> in index.html.

## Structure
    index.html                 homepage
    favicon.ico                browser tab icon
    assets/img/svc_*.webp      booth cover photos (360 / mirror / selfie)
    assets/img/*.webp          gallery photos + poster frames
    assets/video/reel*.mp4     hero showreels, pillarboxed (cycle: 1,2,6,10,5,11,13)
    assets/video/hero.mp4      full showreel ("Watch the showreel" modal)
    assets/video/bmagazine.mp4 magazine booth clip (pillarboxed)
    assets/logos/*.png         all 8 client logos

## Still to wire before go-live
- Lead form opens a pre-filled email to Nufx360activations@gmail.com. Connect submitDate()
  to a real backend (Formspree/Resend) or WhatsApp flow for silent capture.
- Calendly: add your link to the "Check your date" button.
- Analytics: paste your GA4 snippet before </head>.

## Notes
- Prices shown as full figures in Naira. "Most popular" badge on 360 Gold, Mirror Silver,
  Selfie Silver. Mirror extras list applies to the Magic Mirror only.
- Respects prefers-reduced-motion. Fonts: Poppins + Roboto via Google Fonts.
