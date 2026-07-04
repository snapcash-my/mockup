# Static HTML Deployment to Cloudflare Pages

## 🎯 Important: This is a Static HTML Site

**DO NOT** use Wrangler or Workers configuration. This is a simple static HTML site that should be deployed directly to Cloudflare Pages.

## ✅ Correct Cloudflare Pages Settings

### Build Configuration
- **Framework preset**: `None` or `Static HTML`
- **Build command**: Leave empty (no build needed)
- **Build output directory**: `/` (root directory)
- **Root directory**: `/` (root directory)

### Environment Variables
No environment variables required.

## 🚀 Step-by-Step Deployment

### 1. Clean Repository
Ensure your repository only contains:
```
snapcash-retailitics/
├── index.html              # Landing page
├── user-app-mockup.html    # User app mockup
├── merchant-app-mockup.html # Merchant app mockup
├── SnapCash logo.png      # Logo
├── _redirects             # URL redirects
├── README.md              # Documentation
├── DEPLOYMENT.md          # Deployment guide
└── .gitignore             # Git ignore rules
```

### 2. Cloudflare Pages Setup
1. Go to [Cloudflare Dashboard](https://dash.cloudflare.com/)
2. Navigate to **Workers & Pages** → **Pages**
3. Click **Create a project** → **Connect to Git**
4. Select your repository
5. **Configure build settings**:
   ```
   Framework preset: None
   Build command: (leave empty)
   Build output directory: /
   Root directory: /
   ```
6. Click **Save and Deploy**

### 3. Verify Deployment
After deployment, check:
- [ ] Landing page loads correctly
- [ ] Navigation links work
- [ ] App mockups display properly
- [ ] Images load without errors
- [ ] Mobile responsiveness works

## 🚫 What NOT to Do

❌ **DO NOT** use Wrangler CLI  
❌ **DO NOT** create wrangler.toml files  
❌ **DO NOT** set up Workers functions  
❌ **DO NOT** use build commands  

## 🔧 Troubleshooting

### If deployment still fails:
1. **Check file sizes**: Ensure no files > 25MB
2. **Verify .gitignore**: Make sure node_modules is excluded
3. **Clean repository**: Remove any unnecessary files
4. **Clear Cloudflare cache**: In dashboard settings

### Common Issues:
- **Build command error**: Leave build command empty
- **Asset size error**: Remove large files from repository
- **404 errors**: Check that index.html exists in root

## 📊 Expected Results

✅ **Fast deployment** (no build process)  
✅ **Small package size** (~200KB total)  
✅ **Global CDN** distribution  
✅ **Automatic HTTPS**  
✅ **Custom domain** support  

## 🎉 Success Metrics

Your site is successfully deployed when:
- Landing page loads at your Cloudflare Pages URL
- All navigation links work properly
- App mockups are fully functional
- No console errors in browser
- Mobile and desktop views are optimized

---

**Ready for static deployment!** 🚀 No Wrangler, no build process - just pure HTML.
