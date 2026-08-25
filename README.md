# molepack.com

Static review site for EDC / tactical gear. Deployed on Cloudflare Pages.

## Structure

```
├── index.html                          # Homepage
├── best-edc-flashlight-under-50.html   # Article template (first review)
├── about.html                          # About + testing methodology
├── affiliate-disclosure.html           # FTC affiliate disclosure
├── privacy-policy.html                 # Privacy policy (GDPR)
├── css/style.css                       # Shared styles
├── js/main.js                          # Shared scripts
├── sitemap.xml                         # SEO sitemap
├── robots.txt                          # SEO robots
└── _headers                            # Cloudflare cache & security headers
```

## How to publish

This repo is connected to Cloudflare Pages. Every push to `main` triggers an
automatic deployment to molepack.com.

## Adding a new review article

1. Copy `best-edc-flashlight-under-50.html` to a new file (kebab-case, e.g. `best-edc-knives-under-100.html`)
2. Update title, meta description, JSON-LD, content and affiliate links
3. Add the new URL to `sitemap.xml`
4. Commit and push — Cloudflare Pages deploys automatically

## Affiliate links

All affiliate links use `rel="sponsored nofollow"` per FTC guidelines.
