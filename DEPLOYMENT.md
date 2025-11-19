# PowerAI Pitch Deck - Deployment Guide

Deploy your interactive pitch deck to the web for free using GitHub Pages or other platforms.

## 🚀 Quick Deploy Options

### Option 1: GitHub Pages (Recommended - FREE)
**Advantages:** Free, custom domain, version control, easy updates

### Option 2: Netlify (FREE)
**Advantages:** Drag-and-drop, instant deploy, automatic HTTPS

### Option 3: Vercel (FREE)
**Advantages:** Fast deployment, serverless, global CDN

---

## 📦 Option 1: GitHub Pages Deployment

### Step 1: Create a New Repository

1. Go to [GitHub.com](https://github.com)
2. Click **"New Repository"** (green button)
3. Repository settings:
   - **Name:** `powerai-pitch-deck`
   - **Description:** "PowerAI - Renewable Energy Management Platform Pitch Deck"
   - **Visibility:** Public ✓
   - **Initialize:** Don't check any boxes
4. Click **"Create Repository"**

### Step 2: Upload Pitch Deck Files

**Option A: Using GitHub Web Interface**
1. In your new repository, click **"uploading an existing file"**
2. Drag and drop `index.html` from the `pitch-deck` folder
3. Add commit message: "Initial pitch deck upload"
4. Click **"Commit changes"**

**Option B: Using Git Command Line**
```powershell
# Navigate to pitch-deck folder
cd C:\Users\OnePower\AI-For-Software-Engineering-Final-Project\pitch-deck

# Initialize Git repository
git init

# Add remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/powerai-pitch-deck.git

# Add files
git add index.html

# Commit
git commit -m "Initial pitch deck upload"

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **"Settings"** tab
3. Scroll down to **"Pages"** in left sidebar
4. Under **"Source"**:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **"Save"**
6. Wait 1-2 minutes for deployment

### Step 4: Access Your Pitch Deck

Your pitch deck will be available at:
```
https://YOUR_USERNAME.github.io/powerai-pitch-deck/
```

**Example:**
```
https://hlomohangcue.github.io/powerai-pitch-deck/
```

### Step 5: Share Your Deck

Share the URL:
- Add to your email signature
- Include in LinkedIn profile
- Share with investors
- Add to business cards

---

## 📦 Option 2: Netlify Deployment

### Step 1: Sign Up for Netlify

1. Go to [netlify.com](https://www.netlify.com)
2. Sign up with GitHub account (recommended)
3. Authorize Netlify access

### Step 2: Deploy

**Method A: Drag and Drop**
1. Click **"Add new site"** → **"Deploy manually"**
2. Drag the `pitch-deck` folder into the upload area
3. Wait for deployment (30-60 seconds)
4. Your site is live!

**Method B: GitHub Integration**
1. Click **"Add new site"** → **"Import from Git"**
2. Choose GitHub
3. Select `powerai-pitch-deck` repository
4. Settings:
   - Build command: (leave empty)
   - Publish directory: (leave empty if index.html is in root)
5. Click **"Deploy site"**

### Step 3: Custom Domain (Optional)

1. Go to **Site settings** → **Domain management**
2. Click **"Add custom domain"**
3. Follow instructions to configure DNS
4. Free subdomain provided: `your-site-name.netlify.app`

### Your Netlify URL
```
https://your-site-name.netlify.app
```

---

## 📦 Option 3: Vercel Deployment

### Step 1: Sign Up for Vercel

1. Go to [vercel.com](https://vercel.com)
2. Sign up with GitHub account
3. Authorize Vercel access

### Step 2: Deploy

1. Click **"New Project"**
2. **Import Git Repository:**
   - Select your GitHub repository
   - Or drag and drop the `pitch-deck` folder
3. Settings:
   - Framework Preset: Other
   - Build Command: (leave empty)
   - Output Directory: (leave empty)
4. Click **"Deploy"**
5. Wait 30-60 seconds

### Your Vercel URL
```
https://your-project-name.vercel.app
```

---

## 🔗 Custom Domain Setup

### Using Your Own Domain

If you own a domain (e.g., `powerai.co.ls`):

#### For GitHub Pages:
1. Add file `CNAME` to repository with your domain:
   ```
   pitch.powerai.co.ls
   ```
2. In domain registrar, add DNS records:
   ```
   Type: CNAME
   Host: pitch
   Value: YOUR_USERNAME.github.io
   ```

#### For Netlify/Vercel:
1. Go to domain settings in platform
2. Add your custom domain
3. Follow DNS configuration instructions
4. SSL certificate automatically generated

---

## 🎨 Customization Before Deployment

### Update Contact Information

Open `index.html` and find **Slide 12** (bottom of file):

```html
<p style="margin-top: 3rem; font-size: 1.3rem;">
    📧 <span class="highlight">YOUR_EMAIL@example.com</span><br>
    🌐 <span class="highlight">your-website.com</span>
</p>
```

Replace with your actual contact info.

### Update Live Demo Link

Find this line in Slide 12:
```html
<a href="https://powerai-lesotho.streamlit.app" target="_blank" class="cta-button">View Live Demo</a>
```

Ensure the URL is correct.

### Update GitHub Link

Find this line in Slide 12:
```html
<a href="https://github.com/Hlomohangcue/PLP-Final-Project-PowerAI" target="_blank" class="cta-button">View on GitHub</a>
```

Update with your repository URL.

---

## 📊 Adding Analytics (Optional)

### Google Analytics

Add before `</head>` tag in `index.html`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

Replace `GA_MEASUREMENT_ID` with your tracking ID.

---

## 🔄 Updating Your Pitch Deck

### For GitHub Pages:

```powershell
# Navigate to pitch-deck folder
cd C:\Users\OnePower\AI-For-Software-Engineering-Final-Project\pitch-deck

# Make your changes to index.html

# Commit changes
git add index.html
git commit -m "Update pitch deck content"
git push origin main

# Changes live in 1-2 minutes
```

### For Netlify/Vercel:

**If using GitHub integration:**
- Just push to GitHub (same as above)
- Automatic deployment triggers

**If using drag-and-drop:**
- Go to your site dashboard
- Click **"Deploys"**
- Drag updated folder to deploy new version

---

## 📱 Mobile Optimization

The pitch deck is already responsive, but test on:

### Testing Tools:
1. **Chrome DevTools:**
   - Right-click → Inspect
   - Toggle device toolbar (Ctrl+Shift+M)
   - Test different screen sizes

2. **Online Tools:**
   - [Responsive Design Checker](https://responsivedesignchecker.com/)
   - [BrowserStack](https://www.browserstack.com/)

### Mobile Features:
- ✅ Touch swipe navigation
- ✅ Responsive font sizes
- ✅ Optimized button sizes
- ✅ Single column layout on small screens

---

## 🖨️ Creating PDF Version

### For Offline Presentations or Email:

1. Open `index.html` in Google Chrome
2. Press `Ctrl+P` (Print)
3. Settings:
   - Destination: **Save as PDF**
   - Layout: **Landscape**
   - Pages: **All**
   - Margins: **None**
   - Background graphics: **✓ Checked**
4. Click **"Save"**

**Result:** Each slide becomes a PDF page (12 pages total)

---

## 🎥 Creating Video Version

### Using Screen Recording:

1. Open pitch deck in browser (fullscreen F11)
2. Use screen recording software:
   - **Windows:** Xbox Game Bar (Win+G)
   - **OBS Studio** (free, powerful)
3. Navigate through slides slowly
4. Add voiceover narration
5. Export as MP4

### Video Settings:
- Resolution: 1920x1080 (Full HD)
- Frame rate: 30fps
- Audio: 128kbps or higher

**Use for:**
- Email attachments
- Social media promotion
- Website embedding
- Investor outreach

---

## 🔒 Security & Privacy

### Public Deployment Considerations:

**What to Include:**
- ✅ Company overview
- ✅ Product features
- ✅ Market opportunity
- ✅ Contact information

**What to Exclude:**
- ❌ Detailed financial projections
- ❌ Customer names (without permission)
- ❌ Proprietary technology details
- ❌ Sensitive business metrics

### Private Sharing:
If you need to keep deck private:
1. **Password protect** (Netlify/Vercel have options)
2. **Use unlisted URL** (share link only with investors)
3. **Create PDF** and share via secure file sharing

---

## 📈 Tracking Engagement

### Netlify Analytics:
- Built-in analytics (paid feature)
- Track page views, unique visitors
- See referral sources

### Custom Solution:
Add simple view counter using:
- **Counter API** (free): [countapi.xyz](https://countapi.xyz/)
- **Google Analytics** (free)
- **Plausible Analytics** (privacy-focused)

---

## 🐛 Troubleshooting

### Deployment Issues

**GitHub Pages not showing:**
- Check Settings → Pages is enabled
- Ensure `index.html` is in root or specified folder
- Wait 5 minutes for DNS propagation
- Try incognito mode (clear cache)

**Netlify/Vercel errors:**
- Check build logs for errors
- Ensure `index.html` exists in uploaded folder
- Try redeploying
- Contact support if persists

**Styling looks broken:**
- Ensure complete HTML file uploaded
- Check browser console for errors (F12)
- Clear browser cache (Ctrl+Shift+R)
- Test in different browsers

### Navigation Not Working

**Keyboard shortcuts fail:**
- Ensure JavaScript is enabled
- Check browser console for errors
- Try different browser

**Mobile swipe not working:**
- Test on actual device (not just emulator)
- Check touch events in developer tools
- Update to latest browser version

---

## ✅ Pre-Launch Checklist

Before sharing your pitch deck:

- [ ] All links work and point to correct URLs
- [ ] Contact information is current
- [ ] Statistics are up-to-date
- [ ] No spelling/grammar errors
- [ ] Tested on desktop browser
- [ ] Tested on mobile device
- [ ] Tested navigation (arrows, touch)
- [ ] PDF backup created
- [ ] Analytics added (optional)
- [ ] Custom domain configured (optional)
- [ ] Shared with team for feedback
- [ ] Emergency contact info available

---

## 🎯 Best Practices

### For Investor Presentations:
1. **Send ahead:** Email link before meeting
2. **Present live:** Use during pitch (not just PDF)
3. **Follow up:** Include link in thank-you email
4. **Track views:** Use analytics to see engagement
5. **Update regularly:** Keep statistics current

### For Public Promotion:
1. **Social media:** Share on LinkedIn, Twitter
2. **Website:** Embed or link from your site
3. **Email signature:** Add link to signature
4. **Business cards:** Include QR code to deck
5. **Pitch competitions:** Submit as entry material

---

## 📞 Support

### Need Help?

**For technical issues:**
- GitHub Pages: [GitHub Pages Docs](https://docs.github.com/pages)
- Netlify: [Netlify Support](https://www.netlify.com/support/)
- Vercel: [Vercel Docs](https://vercel.com/docs)

**For customization:**
- Edit `index.html` directly
- Basic HTML/CSS knowledge helpful
- Search "HTML tutorial" for learning resources

**For design changes:**
- Consider hiring designer on Fiverr
- Use Canva for alternative format
- Keep it simple and professional

---

## 🎉 You're Ready to Deploy!

Choose your deployment method and follow the steps above. Your pitch deck will be live in minutes!

**Recommended for beginners:** GitHub Pages
**Fastest deployment:** Netlify drag-and-drop
**Most features:** Vercel

---

**Last Updated:** November 19, 2025
**Version:** 1.0
**For:** PowerAI Pitch Deck Deployment
