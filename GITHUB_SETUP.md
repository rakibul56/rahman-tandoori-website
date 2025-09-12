# GitHub Setup Guide for Rahman's Tandoori Website

## 🚀 Quick GitHub Upload Steps

### Option 1: Using GitHub Web Interface (Easiest)

1. **Create Repository**
   - Go to [github.com](https://github.com)
   - Click the green "New" button or "+" icon
   - Repository name: `rahman-tandoori-website`
   - Description: `Official website for Rahman's Tandoori Indian Restaurant in Landshut, Germany`
   - Make it **Public**
   - ✅ Check "Add a README file"
   - Click "Create repository"

2. **Upload Files**
   - In your new repository, click "uploading an existing file"
   - Drag and drop ALL files from your `RahmanTandoory` folder:
     ```
     index.html
     styles.css
     script.js
     logo.png
     tranparent_logo.png
     vercel.json
     package.json
     DEPLOYMENT_GUIDE.md
     DNS_QUICK_REFERENCE.md
     ```
   - Commit message: "Initial upload of Rahman's Tandoori website"
   - Click "Commit changes"

### Option 2: Using Git Commands (Advanced)

1. **Install Git** (if not installed)
   - Download from [git-scm.com](https://git-scm.com)

2. **Initialize Repository**
   ```bash
   cd "C:\Users\rakib\Desktop\RahmanTandoory"
   git init
   git add .
   git commit -m "Initial commit - Rahman's Tandoori website"
   ```

3. **Connect to GitHub**
   ```bash
   git remote add origin https://github.com/YOUR_USERNAME/rahman-tandoori-website.git
   git branch -M main
   git push -u origin main
   ```

## ✅ Verification

After upload, your GitHub repository should contain:
- ✅ index.html
- ✅ styles.css  
- ✅ script.js
- ✅ logo.png
- ✅ tranparent_logo.png
- ✅ vercel.json
- ✅ package.json
- ✅ DEPLOYMENT_GUIDE.md
- ✅ DNS_QUICK_REFERENCE.md
- ✅ README.md (auto-generated)

## 🔗 Next Steps

1. **Copy Repository URL** - You'll need this for Vercel
2. **Go to Vercel** - Follow the DEPLOYMENT_GUIDE.md
3. **Connect Domain** - Update DNS in GoDaddy

Your repository URL will be:
`https://github.com/YOUR_USERNAME/rahman-tandoori-website`

## 🆘 Need Help?

- **GitHub Help**: [docs.github.com](https://docs.github.com)
- **Video Tutorials**: Search "how to upload files to GitHub" on YouTube
- **Alternative**: Use GitHub Desktop app for easier file management