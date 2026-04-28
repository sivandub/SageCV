# Sivan Dubinsky — Sage BDR Resume Site

A single-page resume site built for the Sage Toronto BDR application.

Plain HTML / CSS / JS. No build step.

## Files

```
.
├── index.html        Main page (all content)
├── styles.css        Sage-themed styling (#00dc06)
├── script.js         Scroll reveals + active nav highlighting
├── netlify.toml      Netlify config (publishes from project root)
├── _redirects        Netlify routing fallback
├── robots.txt        Crawler rules
└── README.md         This file
```

## Deploy to Netlify — three options

### Option 1: Drag-and-drop (fastest, ~30 seconds)

1. Go to https://app.netlify.com/drop
2. Drag this entire folder onto the page
3. Netlify gives you a random subdomain like `gleaming-pony-123.netlify.app` — done

### Option 2: Connect a Git repo (recommended for ongoing edits)

1. Push this folder to a GitHub repo
2. In Netlify: **Add new site → Import an existing project → GitHub**
3. Pick the repo. Build command: leave blank. Publish directory: `.`
4. Click **Deploy**. Future pushes to `main` redeploy automatically.

### Option 3: Netlify CLI (for power users)

```bash
npm install -g netlify-cli
cd "Resume Website - Sales"
netlify deploy --prod --dir=.
```

## Custom domain

Once deployed, in Netlify go to **Domain settings → Add custom domain**.
Point a domain (e.g. `sivandubinsky.com`) at Netlify's DNS or use a CNAME.

## Editing

Everything lives in `index.html`. Search for the section you want — `<!-- HERO -->`, `<!-- WHY SAGE -->`, etc. — and edit the copy in place.

To swap colors: change the `--sage`, `--sage-dark`, `--sage-deep`, and `--sage-tint` variables at the top of `styles.css`.
