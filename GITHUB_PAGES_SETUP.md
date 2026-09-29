# 🚀 GitHub Pages Deployment Guide

This is a static website ready to deploy on GitHub Pages!

## Quick Start (5 minutes)

### Step 1: Create a GitHub Repository
1. Go to [github.com/new](https://github.com/new)
2. Create a new repository named: **`your-username.github.io`**
   - Replace `your-username` with your actual GitHub username
   - Example: `sananayyab.github.io`
3. Make it **Public**
4. Click "Create repository"

### Step 2: Upload Files
Choose ONE method below:

#### **Option A: Using Git (Recommended)**
```bash
# Clone your repository
git clone https://github.com/your-username/your-username.github.io.git
cd your-username.github.io

# Copy all files from this folder to your repo folder
# (Copy everything: index.html, _next folder, etc.)

# Push to GitHub
git add .
git commit -m "Initial portfolio commit"
git push -u origin main
```

#### **Option B: GitHub Web UI (Easiest)**
1. Go to your repository on GitHub
2. Click "Add file" → "Upload files"
3. Drag & drop all files from this folder (index.html, _next, about, services, etc.)
4. Commit changes

#### **Option C: GitHub Desktop**
1. Download [GitHub Desktop](https://desktop.github.com)
2. Clone your repository
3. Copy files to the cloned folder
4. Commit and push

### Step 3: Enable GitHub Pages (if needed)
1. Go to repository **Settings** → **Pages**
2. Source should be set to **"Deploy from a branch"**
3. Select **`main`** branch
4. Click Save

### Step 4: Visit Your Site! 🎉
Your site will be live at: **`https://your-username.github.io`**

---

## Folder Structure

```
├── index.html              (Homepage)
├── about/index.html        (About page)
├── services/index.html     (Services page)
├── portfolio/index.html    (Portfolio page)
├── contact/index.html      (Contact page)
├── content-strategy/index.html
├── ai-marketing/index.html
├── _next/                  (JavaScript & CSS files - DO NOT DELETE)
├── favicon.ico
└── .nojekyll              (Important for GitHub Pages)
```

---

## Customization

### Update Site Information
The site content is hardcoded in the HTML. To customize:

1. **Edit Contact Info**: Search for `hello@sananayyab.com` in `index.html`, `contact/index.html`
2. **Edit WhatsApp**: Search for `+923012345678` in HTML files
3. **Edit Social Links**: Search for social URLs (linkedin.com, instagram.com, etc.)

### Update Services/Portfolio
Edit the service and project details directly in the HTML files:
- `services/index.html` - Service descriptions
- `portfolio/index.html` - Project case studies

---

## Troubleshooting

### Site not showing?
- Wait 1-2 minutes after push (first deploy takes longer)
- Check Settings → Pages to verify deployment status
- Clear browser cache (Ctrl+Shift+Delete or Cmd+Shift+Delete)

### Styles not loading?
- Don't delete the `_next` folder - it contains all CSS and JavaScript
- Make sure all files are uploaded, not just HTML files

### Links not working?
- All links are relative paths - they should work if files are structured correctly
- Check that each folder has an `index.html` file

---

## Custom Domain (Optional)

To use your own domain (sananayyab.com):

1. Go to **Settings** → **Pages**
2. Under "Custom domain", enter your domain name
3. Add DNS records to your domain provider (follow GitHub's instructions)
4. GitHub will provide a SSL certificate automatically

---

## Next Steps

### Make Changes Later
Edit HTML files and push changes:
```bash
git add .
git commit -m "Update portfolio content"
git push
```

Changes appear live in 1-2 minutes!

### Add More Pages
1. Create a new folder: `new-page/`
2. Create `new-page/index.html` inside it
3. Add links from other pages to this new page

---

## Support

- GitHub Pages Docs: https://pages.github.com
- GitHub Help: https://docs.github.com/pages
- Built with Next.js & Tailwind CSS ✨
