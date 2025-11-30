# Boply Landing Page

A modern, conversion-optimized landing page for Boply.

## Quick Deploy to Vercel

### Option 1: Vercel CLI (Fastest)

```bash
# Install Vercel CLI if you haven't
npm i -g vercel

# Navigate to this folder
cd landing-page

# Deploy
vercel

# For production
vercel --prod
```

### Option 2: Vercel Dashboard

1. Go to [vercel.com/new](https://vercel.com/new)
2. Import this folder (or push to GitHub first)
3. Click Deploy
4. Done!

### Option 3: GitHub + Vercel

1. Push this folder to a GitHub repo
2. Connect repo to Vercel
3. Auto-deploys on every push

## Custom Domain Setup

After deploying:

1. Go to your Vercel project → Settings → Domains
2. Add `boply.io` (or your domain)
3. Update DNS records as shown
4. SSL is automatic

## Recommended Domain Structure

```
boply.io         → This landing page
app.boply.io     → Your React app
```

## Files Included

```
landing-page/
├── index.html      # The landing page
├── vercel.json     # Vercel configuration
└── README.md       # This file
```

## Customization Checklist

Before going live, update:

- [ ] Replace placeholder app screenshot
- [ ] Update social media links (@boplyapp)
- [ ] Add real testimonials
- [ ] Connect email capture to your system
- [ ] Add analytics (Google Analytics, Mixpanel, etc.)
- [ ] Create /privacy and /terms pages
- [ ] Add favicon/og-image files

## Adding Analytics

Add before `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXX');
</script>
```

## Adding Email Capture

Replace the CTA buttons with a form, or use:
- ConvertKit
- Mailchimp
- Buttondown
- Loops

## Performance

This page is already optimized:
- Single HTML file (no build step)
- Tailwind via CDN (cached globally)
- No heavy JS frameworks
- Optimized fonts (Inter)
- Mobile-first responsive

Lighthouse score should be 95+.

## Need Help?

The landing page includes:
- Hero with CTA
- Problem/solution sections
- Feature highlights
- Social proof/testimonials
- Pricing comparison
- FAQ accordion
- Final CTA
- Footer with links

All sections are clearly commented in the HTML for easy editing.
