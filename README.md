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

## Design System & Image Licensing

- **Colors, spacing, and components**: See `/styles/site.css` for palette, spacing, and utility classes.
- **Product images**: Place licensed/approved images in `/assets/forwardx/` as:
  - flex-300.jpg, flex-300@2x.jpg, flex-300.webp
  - flex-600.jpg, flex-600@2x.jpg, flex-600.webp
- **Editing**: Update copy in `index.html` (Hero, ProductShowcase, UseCases, ValueProps, Process, Contact).
- **Licensing**: Replace placeholder imagery with properly licensed/approved product photos.
- **Deploy**: Push to the tracked branch; CI/CD host will publish. For GoDaddy DNS, point domain to host (A/CNAME).

**TODO:**
- [ ] Swap `/assets/forwardx/flex-300.jpg`, `flex-300.webp`, `flex-600.jpg`, `flex-600.webp` with licensed product images.