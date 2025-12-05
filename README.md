# DualStar Website

This folder contains the static website for dualstar.app

## Files Structure

```
website/
├── index.html          # Landing page (https://dualstar.app)
├── privacy/
│   └── index.html      # Privacy Policy (https://dualstar.app/privacy)
├── terms/
│   └── index.html      # Terms of Service (https://dualstar.app/terms)
├── support/
│   └── index.html      # Support/FAQ page (https://dualstar.app/support)
└── README.md           # This file
```

## URLs for App Stores

| Purpose | URL |
|---------|-----|
| Privacy Policy | https://dualstar.app/privacy |
| Terms of Service | https://dualstar.app/terms |
| Support URL | https://dualstar.app/support |
| Marketing URL | https://dualstar.app |

## Deployment Options

### Option 1: GitHub Pages (Recommended - Free)

1. Create a new GitHub repository named `dualstar-website` (or any name)

2. Push the website folder contents:
   ```bash
   cd website
   git init
   git add .
   git commit -m "Initial website"
   git remote add origin https://github.com/YOUR_USERNAME/dualstar-website.git
   git push -u origin main
   ```

3. Go to repository Settings > Pages

4. Source: Deploy from branch `main`, folder `/ (root)`

5. Configure custom domain:
   - Enter: `dualstar.app`
   - Check "Enforce HTTPS"

6. In GoDaddy DNS settings, add:
   - Type: `A`, Name: `@`, Value: `185.199.108.153`
   - Type: `A`, Name: `@`, Value: `185.199.109.153`
   - Type: `A`, Name: `@`, Value: `185.199.110.153`
   - Type: `A`, Name: `@`, Value: `185.199.111.153`
   - Type: `CNAME`, Name: `www`, Value: `YOUR_USERNAME.github.io`

7. Wait 10-30 minutes for DNS propagation

### Option 2: Cloudflare Pages (Free)

1. Create Cloudflare account at https://pages.cloudflare.com

2. Connect to GitHub or upload directly

3. Configure custom domain in Cloudflare

### Option 3: Netlify (Free)

1. Create Netlify account at https://netlify.com

2. Drag and drop the `website` folder

3. Configure custom domain

### Option 4: Vercel (Free)

1. Create Vercel account at https://vercel.com

2. Import from GitHub or deploy directly

3. Configure custom domain

## Email Setup

After deploying the website, set up email addresses:

### Required Email Addresses:
- `support@dualstar.app` - General support
- `privacy@dualstar.app` - Privacy requests (GDPR/CCPA)
- `legal@dualstar.app` - Legal inquiries
- `billing@dualstar.app` - Billing questions

### Email Options:

1. **Google Workspace** ($6/user/month): Full email + calendar
2. **Zoho Mail** (Free for 5 users): Basic email
3. **Cloudflare Email Routing** (Free): Forward to existing email
4. **ImprovMX** (Free): Forward to existing email

## Pre-Launch Checklist

- [ ] Website deployed and accessible
- [ ] Privacy Policy URL works: https://dualstar.app/privacy
- [ ] Terms of Service URL works: https://dualstar.app/terms
- [ ] Support URL works: https://dualstar.app/support
- [ ] HTTPS enabled (green lock icon)
- [ ] Email forwarding configured
- [ ] Test email delivery to support@dualstar.app

## Updating Content

To update the website:

1. Edit the HTML files locally
2. Commit and push to GitHub
3. Changes deploy automatically (if using GitHub Pages)

## Notes

- All pages use the same dark theme matching the app
- No external dependencies (pure HTML/CSS/JS)
- Mobile responsive design
- SEO meta tags included
- Entertainment disclaimer prominently displayed

## Contact Info in Documents

The following contact information is used:
- Company: Onner Tech Company Limited
- Support: support@dualstar.app
- Privacy: privacy@dualstar.app
- Legal: legal@dualstar.app
- Billing: billing@dualstar.app

