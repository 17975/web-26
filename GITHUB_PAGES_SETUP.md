# GitHub Pages Deployment Guide

Your portfolio is now ready to be hosted on GitHub Pages! Follow these steps:

## Step 1: Create a GitHub Repository

1. Go to [github.com](https://github.com) and sign in
2. Click the **+** icon in the top right → **New repository**
3. Name it: `username.github.io` (replace `username` with your GitHub username)
   - Example: `simonshipanga.github.io`
4. Make it **Public**
5. Click **Create repository**

## Step 2: Upload Your Portfolio

### Option A: Using Git (Recommended)

1. Open PowerShell in your portfolio folder
2. Run these commands:

```powershell
git init
git add .
git commit -m "Initial portfolio commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_USERNAME.github.io.git
git push -u origin main
```

Replace:
- `YOUR_USERNAME` with your GitHub username

### Option B: Upload Files Directly

1. Go to your repository on GitHub
2. Click **Add file** → **Upload files**
3. Drag and drop `index.html` and any other files
4. Click **Commit changes**

## Step 3: Enable GitHub Pages

1. Go to your repository settings
2. Scroll to **Pages** section
3. Under "Build and deployment":
   - Source: Select **Deploy from a branch**
   - Branch: Select **main** folder **/(root)**
4. Click **Save**

Your site will be live at: `https://YOUR_USERNAME.github.io`

## Step 4: Test Your Site

1. Wait 1-2 minutes for deployment
2. Visit `https://YOUR_USERNAME.github.io`
3. Your portfolio should be live!

## Files Included

- **index.html** - Your complete portfolio website

## Customization

To add your actual profile image, video, and PDFs:

1. Upload media files to your repository
2. Update the `src` attributes in `index.html`:
   - Replace profile image URL
   - Replace video src
   - Update link URLs

## Need Help?

- GitHub Pages Docs: https://pages.github.com
- Contact your instructor with the live URL once deployed
