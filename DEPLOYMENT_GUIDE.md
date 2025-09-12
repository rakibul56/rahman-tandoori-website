# Rahman's Tandoori Website - Vercel Deployment Guide

## 📋 Prerequisites

- GitHub account
- Vercel account (free)
- GoDaddy domain: rahmantandoori.de

## 🚀 Step 1: Prepare Your Project for GitHub

1. **Create a GitHub Repository**

   - Go to [GitHub.com](https://github.com)
   - Click "New Repository"
   - Name: `rahman-tandoori-website`
   - Make it Public
   - Click "Create Repository"

2. **Upload Your Files to GitHub**
   - Download GitHub Desktop or use Git commands
   - Upload all your website files:
     - index.html
     - styles.css
     - script.js
     - logo.png
     - tranparent_logo.png
     - vercel.json
     - package.json
     - README.md

## 🌐 Step 2: Deploy to Vercel

1. **Sign Up/Login to Vercel**

   - Go to [vercel.com](https://vercel.com)
   - Sign up with your GitHub account

2. **Import Your Project**

   - Click "New Project"
   - Select "Import Git Repository"
   - Choose your `rahman-tandoori-website` repository
   - Click "Import"

3. **Configure Deployment**

   - Project Name: `rahman-tandoori`
   - Framework Preset: `Other`
   - Root Directory: `./`
   - Build Command: Leave empty (static site)
   - Output Directory: Leave empty
   - Install Command: Leave empty

4. **Deploy**
   - Click "Deploy"
   - Wait for deployment to complete
   - You'll get a URL like: `https://rahman-tandoori.vercel.app`

## 🔗 Step 3: Connect Your GoDaddy Domain

### In Vercel Dashboard:

1. **Add Domain**

   - Go to your project dashboard
   - Click "Settings" → "Domains"
   - Add domain: `rahmantandoori.de`
   - Add domain: `www.rahmantandoori.de`

2. **Get DNS Records**
   - Vercel will show you DNS records to add
   - Copy these values (you'll need them for GoDaddy)

### In GoDaddy Dashboard:

1. **Access DNS Management**

   - Login to your GoDaddy account
   - Go to "My Products" → "Domains"
   - Click "DNS" next to rahmantandoori.de

2. **Add DNS Records**

   **For Root Domain (rahmantandoori.de):**

   - Type: `A`
   - Name: `@`
   - Value: `76.76.19.61` (Vercel's IP)
   - TTL: `3600`

   **For WWW Subdomain:**

   - Type: `CNAME`
   - Name: `www`
   - Value: `cname.vercel-dns.com`
   - TTL: `3600`

3. **Remove Existing Records**
   - Delete any existing A records pointing to @
   - Delete any existing CNAME records for www
   - Keep MX records (for email)

## ⚡ Step 4: Verify and Test

1. **Wait for Propagation**

   - DNS changes can take 24-48 hours
   - Usually works within 1-2 hours

2. **Test Your Domain**

   - Visit: `https://rahmantandoori.de`
   - Visit: `https://www.rahmantandoori.de`
   - Both should show your website

3. **Check SSL Certificate**
   - Vercel automatically provides SSL
   - Your site should have the 🔒 lock icon

## 🔄 Step 5: Future Updates

**To update your website:**

1. Make changes to your files locally
2. Push changes to GitHub
3. Vercel automatically redeploys
4. Your site updates within minutes

## 📱 Step 6: Verify Mobile Responsiveness

Test your website on:

- Desktop browsers
- Mobile phones
- Tablets

## 🛠️ Troubleshooting

**If domain doesn't work:**

1. Check DNS records in GoDaddy
2. Wait longer for propagation
3. Use [dnschecker.org](https://dnschecker.org) to verify

**If images don't load:**

1. Check file paths in HTML
2. Ensure all files are uploaded to GitHub
3. Check case sensitivity in filenames

**SSL Issues:**

- Vercel provides automatic SSL
- Wait 24 hours for full propagation

## 📞 Support

- Vercel Support: [vercel.com/support](https://vercel.com/support)
- GoDaddy Support: [godaddy.com/help](https://godaddy.com/help)

---

## 🎉 Congratulations!

Your Rahman's Tandoori website will be live at:

- **https://rahmantandoori.de**
- **https://www.rahmantandoori.de**

The website is now professional, fast, and automatically scaled globally by Vercel's CDN!
