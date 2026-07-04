# Redeploy Required

The _redirects file has been fixed to resolve the directory listing issue.

## Steps:
1. Push the updated _redirects file to your repository
2. Cloudflare Pages will automatically redeploy
3. The site should now show the landing page instead of directory listing

## What was fixed:
- Removed redirect loop: `/ /index.html 200`
- Kept only app mockup redirects
- Cloudflare Pages now serves index.html by default
