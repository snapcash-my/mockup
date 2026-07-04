# Cloudflare Pages Deployment Guide

## 🚀 Quick Deployment Steps

### 1. Prepare Your Repository

```bash
# Initialize git repository (if not already done)
git init
git add .
git commit -m "Initial commit: SnapCash mockups and landing page"

# Add remote repository
git remote add origin https://github.com/your-username/snapcash-retailitics.git
git push -u origin main
```

### 2. Deploy to Cloudflare Pages

#### Option A: Via Dashboard
1. Go to [Cloudflare Dashboard](https://dash.cloudflare.com/)
2. Navigate to **Workers & Pages** → **Pages**
3. Click **Create a project** → **Connect to Git**
4. Select your repository
5. Configure build settings:
   - **Framework preset**: None
   - **Build command**: Leave empty (static site)
   - **Build output directory**: `/`
   - **Root directory**: `/`
6. Click **Save and Deploy**

#### Option B: Via Wrangler CLI
```bash
# Install Wrangler
npm install -g wrangler

# Login to Cloudflare
wrangler login

# Deploy
wrangler pages deploy . --project-name=snapcash-retailitics
```

### 3. Custom Domain (Optional)

After deployment:
1. Go to your project settings in Cloudflare Dashboard
2. Click **Custom domains**
3. Add your domain (e.g., `snapcash.example.com`)
4. Update DNS records as instructed

## 📁 Deployment Package Structure

```
snapcash-retailitics/
├── index.html                 # Landing page (entry point)
├── user-app-mockup.html       # User app mockup
├── merchant-app-mockup.html    # Merchant app mockup
├── SnapCash logo.png          # Company logo
├── _redirects                 # Cloudflare redirects
├── README.md                  # Project documentation
├── DEPLOYMENT.md              # This deployment guide
├── package.json               # Project metadata
└── docs/                      # Documentation folder
    └── snapcash-screen-catalog.md
```

## ⚡ Performance Optimizations

The site is optimized for Cloudflare Pages with:

- **Static Assets**: All files are static, no server-side processing needed
- **CDN Ready**: Cloudflare's global CDN ensures fast loading worldwide
- **Image Optimization**: Uses external CDN for placeholder images
- **Minified Dependencies**: Uses CDN-hosted Tailwind CSS and Font Awesome

## 🔧 Configuration Files

### `_redirects`
Handles clean URLs and proper routing:
- `/` → `/index.html`
- `/user-app` → `/user-app-mockup.html`
- `/merchant-app` → `/merchant-app-mockup.html`

### `package.json`
Contains project metadata and local development scripts:
- `npm run dev` - Start local development server
- `npm run preview` - Preview built site

## 🌐 Environment Variables

No environment variables required for this static site.

## 📊 Deployment Features

- **Automatic HTTPS**: Free SSL certificate
- **Global CDN**: Fast loading worldwide
- **Instant Rollbacks**: Easy deployment history
- **Custom Domains**: Support for branded URLs
- **Analytics**: Built-in visitor analytics
- **Preview Deployments**: Test changes before going live

## 🚨 Troubleshooting

### Common Issues

1. **404 Errors**
   - Check that `index.html` exists in root
   - Verify `_redirects` file is properly configured

2. **Styling Issues**
   - Ensure Tailwind CSS CDN is accessible
   - Check Font Awesome CDN links

3. **Image Loading**
   - Verify `SnapCash logo.png` exists
   - Check external image URLs are accessible

### Debug Mode

Add `?debug=true` to URL to enable debug information in development.

## 🔄 Continuous Deployment

Set up automatic deployments:

1. **GitHub Integration**: Connect your repository
2. **Branch Settings**: Choose which branches trigger deployments
3. **Preview Deployments**: Automatically preview pull requests

## 📈 Post-Deployment Checklist

- [ ] Landing page loads correctly
- [ ] Navigation links work properly
- [ ] App mockups display correctly
- [ ] Mobile responsiveness tested
- [ ] All images load without errors
- [ ] Forms and interactive elements work
- [ ] SEO meta tags are present
- [ ] Custom domain configured (if applicable)

## 🎉 Success Metrics

Your SnapCash mockup site is successfully deployed when:

✅ Landing page loads at your domain
✅ All navigation links work
✅ App mockups are fully functional
✅ Mobile and desktop views are optimized
✅ Loading time is under 3 seconds
✅ No console errors in browser

---

**Ready to launch!** 🚀 Your SnapCash Decentralized ATM Network mockup is now prepared for Cloudflare Pages deployment.
