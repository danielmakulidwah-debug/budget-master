# 🚀 Budget Master - Deployment Guide

## Quick Deploy to GitHub Pages (5 Minutes)

### Step 1: Create GitHub Account
1. Go to [github.com](https://github.com)
2. Click "Sign up"
3. Choose username (e.g., `danielmakulidwa`)
4. Verify email

### Step 2: Create Repository
1. Click **"+"** → **"New repository"**
2. Repository name: `budget-master`
3. Description: `Personal Finance Management App for Malawians`
4. **Public** (required for free GitHub Pages)
5. ✅ Check "Add a README file"
6. Click **"Create repository"**

### Step 3: Upload Files
Upload these files to your repository:

```
budget-master/
├── index.html
├── add-transaction.html
├── budget.html
├── savings-goals.html
├── manifest.json
├── service-worker.js
├── README.md
└── icons/
    ├── icon-72x72.png
    ├── icon-96x96.png
    ├── icon-128x128.png
    ├── icon-144x144.png
    ├── icon-152x152.png
    ├── icon-192x192.png
    ├── icon-384x384.png
    └── icon-512x512.png
```

**Two ways to upload:**

#### Option A: Web Upload (Easy)
1. Click **"Add file"** → **"Upload files"**
2. Drag all files into the upload area
3. Write commit message: "Initial commit"
4. Click **"Commit changes"**

#### Option B: GitHub Desktop (Recommended)
1. Download [GitHub Desktop](https://desktop.github.com)
2. Clone your repository
3. Copy all files to the folder
4. Commit and push

### Step 4: Enable GitHub Pages
1. Go to repository **Settings**
2. Scroll to **"Pages"** (left sidebar)
3. Source: **"Deploy from a branch"**
4. Branch: **"main"** → **"/ (root)"**
5. Click **"Save"**

### Step 5: Wait for Deployment
- GitHub takes 1-5 minutes to build
- Refresh the Pages section
- You'll see: **"Your site is live at https://danielmakulidwa.github.io/budget-master/"**

---

## 🎨 Creating App Icons

You need 8 icon sizes. Here are your options:

### Option A: Use Icon Generator (Easiest)
1. Go to [realfavicongenerator.net](https://realfavicongenerator.net)
2. Upload a square logo (512x512 recommended)
3. Generate all sizes
4. Download and extract to `icons/` folder

### Option B: Design Your Own
Create a 512x512 icon with:
- **Background**: Green gradient (#22c55e to #3b82f6)
- **Icon**: White wallet/money symbol
- **Text**: Optional "BM" or "Budget Master"

Use tools:
- [Canva](https://canva.com) - Free templates
- [Figma](https://figma.com) - Professional design
- [GIMP](https://gimp.org) - Free Photoshop alternative

Then resize to all required sizes:
- 72x72, 96x96, 128x128, 144x144, 152x152, 192x192, 384x384, 512x512

### Option C: Use Placeholder (Quick Start)
I can generate a simple SVG icon that works for testing.

---

## 📱 Testing Your PWA

### On Desktop (Chrome/Edge):
1. Visit your GitHub Pages URL
2. Look for **"Install"** button in address bar
3. Click to install
4. App opens in standalone window
5. Works offline!

### On Android:
1. Open in Chrome
2. Menu (⋮) → **"Add to Home Screen"**
3. Icon appears on home screen
4. Tap to open like native app
5. Works offline!

### On iPhone/iPad:
1. Open in Safari
2. Share button (square with arrow)
3. **"Add to Home Screen"**
4. Icon appears on home screen
5. Works offline!

---

## ✅ Verification Checklist

After deployment, test:

- [ ] Website loads at your GitHub Pages URL
- [ ] All 4 pages work (Overview, Add Transaction, Budget, Goals)
- [ ] Install prompt appears after 10 seconds
- [ ] Can install to home screen
- [ ] Works offline after first visit
- [ ] Data saves in localStorage
- [ ] Export/backup functions work
- [ ] USSD helper works
- [ ] All icons load correctly

---

## 🔧 Troubleshooting

### "404 Page Not Found"
- Check GitHub Pages is enabled
- Ensure branch is set to `main`
- Wait 5 minutes for deployment
- Check file names (case-sensitive)

### Icons Don't Load
- Verify `icons/` folder exists
- Check file names match manifest.json
- Icons must be PNG format
- Re-upload with correct names

### Install Button Doesn't Appear
- Must be HTTPS (GitHub Pages is automatic)
- manifest.json must be valid JSON
- Icons must exist at specified paths
- Try in Chrome/Edge (best support)

### Offline Mode Not Working
- Service worker needs HTTPS
- GitHub Pages provides HTTPS automatically
- Check browser console for errors
- Try refreshing page twice

---

## 🎯 Custom Domain (Optional)

Want `budgetmaster.com` instead of GitHub Pages URL?

### Steps:
1. Buy domain from:
   - [Namecheap](https://namecheap.com) - $8/year
   - [Google Domains](https://domains.google) - $12/year
   - [Cloudflare](https://cloudflare.com) - $9/year

2. In GitHub Pages settings:
   - Add custom domain: `budgetmaster.com`
   - Wait for DNS check

3. In domain registrar:
   - Add A records:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - Add CNAME record: `www` → `danielmakulidwa.github.io`

4. Wait 24 hours for DNS propagation

---

## 📊 Adding Analytics (Optional)

Track how many people use your app:

### Google Analytics (Free):
1. Go to [analytics.google.com](https://analytics.google.com)
2. Create property
3. Get tracking ID (G-XXXXXXXXXX)
4. Add to `index.html` `<head>`:

```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

---

## 🔄 Updating Your App

### Method 1: Web Upload
1. Go to repository
2. Click on file to edit
3. Click pencil icon (Edit)
4. Make changes
5. Commit changes
6. GitHub Pages auto-updates in 1-2 minutes

### Method 2: GitHub Desktop
1. Make changes locally
2. Commit in GitHub Desktop
3. Push to GitHub
4. Auto-deploys

---

## 🎉 You're Live!

Your app is now:
- ✅ Hosted for FREE forever
- ✅ Available at `https://yourusername.github.io/budget-master`
- ✅ Installable on any device
- ✅ Works 100% offline
- ✅ Auto-updates when you push changes
- ✅ Secured with HTTPS
- ✅ Accessible worldwide

**Share your URL with users in Malawi!**

---

## 💡 Next Steps

1. **Share on social media**
   - Facebook, WhatsApp, Twitter
   - "Try Budget Master - Free personal finance app"

2. **Get feedback**
   - Ask users what they want
   - Fix bugs quickly
   - Add features based on requests

3. **Market locally**
   - Malawi tech groups
   - University students
   - Small business owners

4. **Consider monetization** (later)
   - Premium features
   - Ads (Google AdSense)
   - Donations (Buy Me a Coffee)

---

## 📞 Support

**Need help with deployment?**

**Developer**: Daniel Makulidwa  
**Email**: danielmakulidwah@gmail.com  
**Phone**: +265 886 872 397  
**WhatsApp**: +265 886 872 397

---

## 📝 License

MIT License - Free to use and modify

---

**Built with ❤️ in Malawi**  
© 2026 Budget Master - Daniel Makulidwa