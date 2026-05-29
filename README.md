# BetNinja — Bonus Guide (green design)

Fourth static site: green bonus-guide layout matching the reference screenshot
(brand + pills header, hero with CTA + original casino illustration, content cards,
welcome/no-deposit/codes, promotions table, wagering, claim steps, FAQ). Responsive.

## Files
```
index.html      → bonus guide (links logo.svg + favicon.png + style.css; hero art is inline SVG)
style.css       → all styles (green theme, Saira + Barlow)
logo.svg        → ninja headband-mask logo
logo.png        → raster logo (apple-touch-icon)
favicon.png     → tab icon
go/index.html   → cloaked redirect; /go → partner URL
```

## /go redirect
In-page `/go` links intercepted by JS in index.html; direct hits use go/index.html
(JS replace + meta-refresh, noindex). Change destination in BOTH: `PARTNER_URL`
in index.html and the three occurrences in go/index.html.

## Deploy (GitHub Pages)
Upload all files (keep `go/`), then Settings → Pages → branch `main`, folder `/ (root)`.
For a project page, switch CTA links to `/<repo>/go` so the static fallback works.

## Notes
Honest international version: UK targeting from the source ("Complete Guide for UK Players",
"full UK details", GBP, "© ... UK") removed; currency shown in EUR; the hero illustration is
an original SVG (not a copy of the reference image). Offshore (Anjouan) licence stated
accurately; the disclaimer notes UKGC/GamStop do NOT apply. 18+ / responsible-gambling notes intentional.
