# evanhawkins.com

The void's official website.

## File structure

```
evanhawkins-site/
├── index.html                       # main playground (Y2K chaos)
├── about.html                       # entity dossier
├── work.html                        # project registry (terminal)
├── contact.html                     # transmission shrine
├── now.html                         # current focus snapshot
├── blog.html                        # placeholder
├── archive.html                     # placeholder
├── bitcoinclock.html                # live BTC block clock
├── pocket-oracle-buildplan-v1.html  # codex
├── 404.html                         # lost in the void
├── favicon.svg                      # site icon
├── og-image.png                     # social share card (1200x630)
├── catgirl-cursor.png               # custom cursor sprite
├── robots.txt                       # SEO
└── sitemap.xml                      # SEO
```

## Hidden features

- **Konami code** on the homepage: ↑ ↑ ↓ ↓ ← → ← → B A — spawns floating cat girls + hue shift
- **8 secret zones** hidden around the playground
- **Click EVAN HAWKINS** title for a hue-rotate flash
- **Live BTC block height** in top-right corner (click to open clock)
- **Guestbook** is writable and persists in browser localStorage

## Deployment

### Option A: GitHub Pages (simplest if already on GitHub)
1. Push these files to the root of your `evanhawkins.com` repo
2. Settings → Pages → Deploy from branch → main
3. Add custom domain `evanhawkins.com` in the same settings

### Option B: Cloudflare Pages (faster CDN)
1. https://dash.cloudflare.com → Pages → Create project
2. Direct upload → drag the `evanhawkins-site` folder
3. Custom domains → add `evanhawkins.com`

### Option C: Vercel
1. https://vercel.com/new → import GitHub repo
2. Deploy
3. Settings → Domains → add `evanhawkins.com`

## Things to update before deploy

1. Confirm X handle is `@eviaeai` (or fix in `contact.html`, `blog.html`, `index.html` meta)
2. Replace `og-image.png` with a screenshot if you want a fancier social card
3. Update `now.html` regularly — that's the point of a /now page

## Pre-deploy checklist

- [ ] X handle verified
- [ ] All pages tested locally (open `index.html` in browser, click every portal)
- [ ] Custom domain set up
- [ ] OG card previewed: https://www.opengraph.xyz

## Stack

- Pure HTML/CSS/JS, no build step, no dependencies
- WebGL shader for the DMT tunnel background
- localStorage for guestbook persistence
- mempool.space API for live BTC block height
- Catgirl sprite hosted locally
