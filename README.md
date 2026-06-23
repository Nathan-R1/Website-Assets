# Nathansoftware Website

A static two-page site hosted on AWS behind Cloudflare.

## Pages

| Page | File | Description |
|------|------|-------------|
| Home | `index.html` | Landing page with hero, featured software, about, work/services grid, and news carousel |
| Downloads | `downloads.html` | App catalog (Personal/Business/Pro) with expandable sections and games showcase |

## Structure

```
Website-Assets/
├── index.html           # Home page
├── downloads.html       # Downloads page
├── styles/
│   ├── index.css        # Home page styles
│   └── downloads.css    # Downloads page styles
├── assets/
│   ├── icons/           # App icons (glass.png, esc.png, ic.png, math.png, timer.png, btw.jpg)
│   └── *.jpg/*.png      # Backgrounds, screenshots, and branding assets
└── README.md
```

## Infrastructure

- **Hosting**: AWS (S3 / CloudFront)
- **CDN / DNS**: Cloudflare
- **No build step** — plain HTML, CSS, and JS served statically
- **Asset CDN**: Images/icons served via jsDelivr from the `Nathan-R1/Website-Assets` GitHub repo
