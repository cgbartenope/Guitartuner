# Deployment Guide

This guide will help you deploy the Guitar Tuner Directory to GitHub Pages.

## Prerequisites

- GitHub account
- Git installed on your computer
- Basic knowledge of Git commands

## Option 1: Deploy to GitHub Pages (Recommended)

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and log in
2. Click the **"+"** icon in the top right corner
3. Select **"New repository"**
4. Name your repository (e.g., `guitar-tuner-directory`)
5. Choose **Public** (required for free GitHub Pages)
6. **Do not** initialize with README (we already have one)
7. Click **"Create repository"**

### Step 2: Push Your Code

If you haven't cloned this repository yet:

```bash
# Navigate to where you want the project
cd ~/projects

# Clone the repository
git clone https://github.com/YOUR-USERNAME/guitar-tuner-directory.git
cd guitar-tuner-directory

# Copy all files from this project into the directory
# Then commit
git add .
git commit -m "Initial commit: Guitar Tuner Directory"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/guitar-tuner-directory.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **"Settings"** (top menu)
3. Scroll down to **"Pages"** in the left sidebar
4. Under **"Source"**, select **"main"** branch
5. Keep the folder as **"/ (root)"**
6. Click **"Save"**

### Step 4: Access Your Site

After a few minutes, your site will be live at:
```
https://YOUR-USERNAME.github.io/guitar-tuner-directory/
```

GitHub will show you the URL in the Pages settings.

## Option 2: Deploy to Netlify

### Step 1: Push to GitHub
Follow steps 1-2 from Option 1 above.

### Step 2: Deploy to Netlify

1. Go to [Netlify](https://www.netlify.com/)
2. Sign up or log in
3. Click **"Add new site"** → **"Import an existing project"**
4. Choose **"GitHub"**
5. Authorize Netlify to access your repositories
6. Select your `guitar-tuner-directory` repository
7. Build settings:
   - Build command: (leave empty)
   - Publish directory: (leave empty or set to `/`)
8. Click **"Deploy site"**

Your site will be live at a random Netlify URL (e.g., `random-name-123.netlify.app`)

### Optional: Custom Domain on Netlify

1. Go to **Site settings** → **Domain management**
2. Click **"Add custom domain"**
3. Follow the instructions to configure your DNS

## Option 3: Deploy to Vercel

### Step 1: Push to GitHub
Follow steps 1-2 from Option 1 above.

### Step 2: Deploy to Vercel

1. Go to [Vercel](https://vercel.com/)
2. Sign up or log in with GitHub
3. Click **"Add New"** → **"Project"**
4. Import your `guitar-tuner-directory` repository
5. Configure project:
   - Framework Preset: **Other**
   - Build Command: (leave empty)
   - Output Directory: (leave empty)
6. Click **"Deploy"**

Your site will be live at a Vercel URL (e.g., `guitar-tuner-directory.vercel.app`)

## Option 4: Traditional Web Hosting

If you have traditional web hosting (cPanel, FTP access, etc.):

1. **Download all files** from this project
2. **Upload to your web server** using:
   - FTP client (FileZilla, Cyberduck)
   - cPanel File Manager
   - Your hosting provider's upload method
3. Ensure `index.html` is in the root directory
4. Access your site at your domain

## Custom Domain Setup

### For GitHub Pages:

1. Buy a domain from a registrar (Namecheap, GoDaddy, etc.)
2. In your DNS settings, add a **CNAME record**:
   - Name: `www` (or `@` for root domain)
   - Value: `YOUR-USERNAME.github.io`
3. In your GitHub repo:
   - Go to **Settings** → **Pages**
   - Enter your custom domain
   - Check **"Enforce HTTPS"**

### For Netlify/Vercel:

Follow their custom domain guides (they're well documented and user-friendly).

## Post-Deployment Checklist

After deploying, verify:

- [ ] All sections load correctly
- [ ] Navigation links work
- [ ] External links open in new tabs
- [ ] Responsive design works on mobile
- [ ] Smooth scrolling functions properly
- [ ] Animations trigger correctly
- [ ] No console errors (F12 to check)

## Updating Your Site

After making changes:

```bash
# Make your changes to the files
# Then commit and push

git add .
git commit -m "Description of changes"
git push origin main
```

For GitHub Pages/Netlify/Vercel: Changes deploy automatically!

## Troubleshooting

### GitHub Pages not showing updates?
- Wait 2-5 minutes for changes to deploy
- Check the "Actions" tab for build status
- Clear your browser cache (Ctrl+Shift+R or Cmd+Shift+R)

### CSS/JS not loading?
- Verify all file paths are correct
- Check that files are committed to the repository
- Clear browser cache

### 404 Error?
- Ensure `index.html` is in the root directory
- Check that GitHub Pages is enabled
- Verify the repository is public

### Links not working?
- Make sure you're using relative paths for internal links
- Use `target="_blank"` for external links
- Check that URLs are complete (include `https://`)

## Performance Optimization (Optional)

### Minify CSS
Use a tool like [CSS Minifier](https://cssminifier.com/) to reduce file size.

### Optimize Images
If you add images later, use tools like:
- [TinyPNG](https://tinypng.com/)
- [ImageOptim](https://imageoptim.com/)

### Enable Caching
If using custom hosting, add to `.htaccess`:
```apache
<IfModule mod_expires.c>
  ExpiresActive On
  ExpiresByType text/css "access plus 1 year"
  ExpiresByType text/javascript "access plus 1 year"
</IfModule>
```

## Analytics (Optional)

### Add Google Analytics

1. Create a Google Analytics account
2. Get your tracking ID
3. Add before closing `</head>` tag:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_TRACKING_ID');
</script>
```

## Need Help?

- GitHub Pages docs: https://docs.github.com/en/pages
- Netlify docs: https://docs.netlify.com/
- Vercel docs: https://vercel.com/docs
- Open an issue on the repository

---

Good luck with your deployment! 🚀
