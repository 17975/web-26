# File Organization Guide for GitHub Pages

Your portfolio is now customized to use real files. Here's how to organize them:

## Folder Structure for GitHub Repo

```
username.github.io/
├── index.html                                    (main portfolio page)
├── whatsapp-image.jpg                           (your profile photo)
├── web-video.mp4                                (your demo video)
├── matlab_1.pdf                                 (MATLAB assignments)
├── matlab_2.pdf
└── matlab_3.pdf
```

## File Names to Use

Make sure your files have these **exact** names:

| Current File | Upload Name | Source |
|---|---|---|
| WhatsApp Image 2026-06-13 at 18.00.09 (1).jpeg | `whatsapp-image.jpg` | Your Downloads folder |
| web video.mp4 | `web-video.mp4` | Your Downloads folder |
| matlab_1.pdf.pdf | `matlab_1.pdf` | From your Downloads |
| matlab_2.pdf.pdf | `matlab_2.pdf` | From your Downloads |
| matlab_3.pdf.pdf | `matlab_3.pdf` | From your Downloads |

## How to Upload to GitHub

### Option 1: GitHub Web Interface (Easiest)

1. Create your repository: `username.github.io`
2. Click **Add file** → **Upload files**
3. Upload all files at once (Ctrl+A to select multiple)
4. Commit the files

### Option 2: Using Git Command Line

```powershell
cd C:\Users\224164090\Downloads\app_default_26_06_13_13_31_53 (2)

# Copy your media files here and rename them
# Copy index.html here

# Then run:
git init
git add .
git commit -m "Portfolio with media files"
git branch -M main
git remote add origin https://github.com/USERNAME/USERNAME.github.io.git
git push -u origin main
```

## Files Already Updated

✅ **index.html** - Updated to reference:
- `whatsapp-image.jpg` for your profile photo
- `web-video.mp4` for your video
- `matlab_1.pdf`, `matlab_2.pdf`, `matlab_3.pdf` for MATLAB assignments

## After Upload

1. Wait 1-2 minutes for deployment
2. Visit `https://USERNAME.github.io`
3. Test all links:
   - Profile image should load
   - Video should play
   - PDF buttons should open files

## Need to Add More PDFs?

The portfolio has 3 PDF cards but you mentioned 8 MATLAB files. To add more:

1. Edit `index.html`
2. Copy this block and paste it again in the PDF grid:

```html
<div class="pdf-card">
    <div class="pdf-card-header">
        <div>
            <div class="pdf-card-title">MATLAB Assignment X</div>
            <div class="pdf-card-filename">matlab_X.pdf</div>
        </div>
        <span class="pdf-card-pages">X pages</span>
    </div>
    <div class="pdf-card-preview">
        Description of the assignment...
    </div>
    <a href="matlab_X.pdf" class="btn btn-primary" style="width: 100%; justify-content: center;">📄 Open PDF</a>
</div>
```

3. Replace `X` with the number and upload the corresponding PDF file

Let me know if you need help with the upload or adding more PDFs!
