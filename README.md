# ADSA StudioDesign Blog — Static Site

Zero-cost SEO blog. No build step, no external dependencies (system fonts only), no accounts needed.

## What's here

- `index.html` — homepage with all 5 article cards + excerpts
- `articles/*.html` — the 5 SEO articles, one per product
- `assets/style.css` — shared stylesheet (navy `#0A2540` / amber `#E8A33D`)
- `sitemap.xml` / `robots.txt` — SEO plumbing

Every page has: `<title>`, meta description with its target keyword, Open Graph tags, exactly one `<h1>`, semantic HTML, and a "Get the spreadsheet on Etsy" CTA button linking to the correct listing. Mobile-responsive.

## Before deploying — one required edit

Replace every `YOUR-DOMAIN-HERE` with your real domain. It appears in:

- `sitemap.xml` (6 URLs + a reminder comment)
- `robots.txt` (the Sitemap line)
- the `og:url` tag on each page

## Preview locally

```bash
cd blog-site && python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy free (when ready)

Drag-and-drop the `blog-site/` folder contents onto **Netlify Drop**, **Cloudflare Pages**, or push to a **GitHub Pages** repo. No build command, no config — it's plain static files.

**Status: built and validated. NOT deployed anywhere, no accounts created.**
