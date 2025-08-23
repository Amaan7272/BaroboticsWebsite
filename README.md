# BaroboticsWebsite

## How we deploy & update

Edit homepage content in `index.html`.

**Run locally:**
Just open `index.html` in your browser. No build step required.

**Edit points:**
- Main content: `index.html`
- Styles: inlined in `<head>` of `index.html`
- Images: place in `public/` (reference as `/public/yourimage.jpg`)

**Push changes:**
```
git add -A
git commit -m "chore: update landing content"
git push
```

DNS/hosting is managed separately (domain: GoDaddy). This repo holds the site code only.