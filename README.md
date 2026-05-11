# YeahDev

> Practical articles to help you build and grow your business.

Live at [yeahdev.com](https://yeahdev.com)

## Structure

```
yeahdev/
├── index.html              # Homepage
├── css/
│   ├── main.css            # Global styles (header, footer, cards)
│   └── article.css         # Article page styles
├── articles/
│   └── best-free-ai-video-tools-2026.html
└── README.md
```

## Deploying to GitHub Pages

1. Create a new GitHub repo named `yeahdev` (or your username.github.io)
2. Push all files to the `main` branch
3. Go to **Settings → Pages → Source** → select `main` branch, root `/`
4. GitHub will publish it at `https://<yourusername>.github.io/yeahdev`

## Connecting to Cloudflare Pages (with custom domain)

1. Push repo to GitHub as above
2. In Cloudflare dashboard → **Pages → Create a project → Connect to Git**
3. Select your GitHub repo
4. Build settings:
   - **Framework preset:** None
   - **Build command:** *(leave empty)*
   - **Build output directory:** `/` (or `.`)
5. Deploy — Cloudflare will give you a `*.pages.dev` URL
6. Add your custom domain `yeahdev.com` under **Custom Domains**
7. Update your domain's nameservers to Cloudflare (or add a CNAME)

## Adding Articles

1. Duplicate `articles/best-free-ai-video-tools-2026.html`
2. Update the title, meta, breadcrumb, and content
3. Add a new `<article class="card">` block in `index.html`
4. Commit and push — Cloudflare Pages auto-deploys on every push

## Fonts

Uses Google Fonts (loaded via CDN):
- **Playfair Display** — headlines
- **DM Sans** — body text
- **DM Mono** — labels, tags, code
