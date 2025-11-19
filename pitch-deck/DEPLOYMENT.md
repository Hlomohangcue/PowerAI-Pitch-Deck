# PowerAI Pitch Deck - Deployment Guide

Deploy your interactive pitch deck to the web for free using GitHub Pages or other platforms.

## ⚡ Quick Start Guide (5 Minutes)

**Already familiar with GitHub?** Here's the express version:

1. Create a new public repository on GitHub
2. Upload `index.html` to the repository root
3. Go to Settings → Pages
4. Set Source to "Deploy from a branch", Branch to "main", Folder to "/ (root)"
5. Click Save and wait 2 minutes
6. Visit `https://YOUR_USERNAME.github.io/REPO_NAME/`
7. Done! 🎉

**Need more detailed guidance?** See the complete step-by-step guide below.

---

## 🚀 Deployment Options Comparison

### Option 1: GitHub Pages (Recommended - FREE) ⭐
**Advantages:** 
- ✅ Completely FREE hosting forever
- ✅ Custom domain support (yourname.github.io)
- ✅ Built-in version control with Git
- ✅ Easy updates - just push to GitHub
- ✅ Automatic HTTPS/SSL certificates
- ✅ No credit card required
- ✅ Perfect for pitch decks and presentations
- ✅ Professional URL for investor communications
- ✅ No time limits or bandwidth restrictions

**Best for:** Professional pitch decks, portfolios, documentation

### Option 2: Netlify (FREE)
**Advantages:** Drag-and-drop, instant deploy, automatic HTTPS

**Best for:** Quick tests, drag-and-drop deployment

### Option 3: Vercel (FREE)
**Advantages:** Fast deployment, serverless, global CDN

**Best for:** Web applications with serverless functions

---

## 📦 OPTION 1: GITHUB PAGES DEPLOYMENT (DETAILED GUIDE)

This is the **RECOMMENDED** method for deploying your PowerAI Pitch Deck. Follow these steps carefully.

---

### 🎯 What You'll Achieve:
By the end of this guide, your pitch deck will be:
- Live on the internet at a professional URL
- Accessible 24/7 from anywhere in the world
- Easy to share with investors and stakeholders
- Simple to update whenever you need to make changes

**Estimated Time:** 10-15 minutes (first time setup)

**Prerequisites:**
- A GitHub account (free) - [Sign up here](https://github.com/join) if you don't have one
- Your pitch deck files (index.html) ready to upload

---

### 📋 STEP-BY-STEP GUIDE

### Step 1: Prepare Your GitHub Account

**If you already have a GitHub account:**
- Go to [GitHub.com](https://github.com) and sign in
- Skip to Step 2

**If you need to create an account:**
1. Go to [GitHub.com](https://github.com)
2. Click **"Sign up"** in the top right
3. Enter your email, create a password, and choose a username
   - **TIP:** Choose a professional username (e.g., "hlomohangcue" or "powerai-lesotho")
   - This username will be part of your pitch deck URL
4. Verify your email address
5. You're ready to proceed!

---

### Step 2: Create a New Repository for Your Pitch Deck

A repository is like a folder on GitHub that will store your pitch deck files.

1. **Sign in to GitHub** and go to your homepage
2. Click the **green "New"** button (or go to https://github.com/new)
3. **Configure your repository:**
   
   **Repository name:** `PowerAI-Pitch-Deck` or `powerai-pitch-deck`
   - This will be part of your URL
   - Use lowercase and hyphens for best compatibility
   - **Your URL will be:** `https://YOUR_USERNAME.github.io/powerai-pitch-deck/`
   
   **Description:** (optional but recommended)
   ```
   PowerAI - AI-Powered Renewable Energy Management Platform - Interactive Pitch Deck
   ```
   
   **Visibility:** ⚠️ Choose **"Public"**
   - GitHub Pages only works with public repos on free accounts
   - Your pitch deck will be visible to anyone with the link
   - This is normal for pitch decks - you WANT investors to see it
   
   **Initialize repository:**
   - ❌ **DO NOT** check "Add a README file"
   - ❌ **DO NOT** add .gitignore
   - ❌ **DO NOT** choose a license
   - Leave all checkboxes unchecked (we'll add files manually)

4. Click **"Create repository"** (green button at bottom)

**Result:** You now have an empty repository ready for your pitch deck!

---

### Step 3: Upload Your Pitch Deck Files

Now you'll upload your pitch deck to GitHub. Choose the method that's easiest for you:

---

#### 🖱️ **METHOD A: Web Upload (EASIEST - Recommended for Beginners)**

This method uses only your web browser - no command line needed!

1. **You should see a setup screen** with several options
   - If you don't see this, go to your repository: `https://github.com/YOUR_USERNAME/powerai-pitch-deck`

2. **Look for the link** that says **"uploading an existing file"**
   - It's in the middle of the page, in a sentence like:
   - "Get started by creating a new file or uploading an existing file"
   - Click on **"uploading an existing file"**

3. **Upload your pitch deck:**
   - You'll see a drag-and-drop area
   - **Option 1:** Drag `index.html` from your computer and drop it here
   - **Option 2:** Click "choose your files" and browse to select `index.html`
   - **File location:** The file is in the `pitch-deck` folder of this repository

4. **Add a commit message:**
   - In the text box at the bottom, enter:
   ```
   Initial pitch deck upload
   ```
   - This describes what you're doing (uploading the deck)

5. **Commit (save) the file:**
   - Click the green **"Commit changes"** button
   - Wait a few seconds for the upload to complete

**Result:** Your `index.html` file is now on GitHub! ✅

---

#### 💻 **METHOD B: Git Command Line (For Advanced Users)**

If you're comfortable with command line tools, this method gives you more control.

**Prerequisites:**
- Git must be installed on your computer ([Download Git](https://git-scm.com/downloads))
- Basic familiarity with command line/terminal

**Steps:**

1. **Open your terminal or command prompt**
   - Windows: Search for "Command Prompt" or "PowerShell"
   - Mac: Open "Terminal" from Applications
   - Linux: Open your terminal app

2. **Navigate to your pitch-deck folder:**
   ```bash
   # Example - adjust the path to where YOUR files are located:
   cd /path/to/PowerAI-Pitch-Deck/pitch-deck
   
   # Windows example:
   # cd C:\Users\YourName\PowerAI-Pitch-Deck\pitch-deck
   
   # Mac/Linux example:
   # cd ~/Documents/PowerAI-Pitch-Deck/pitch-deck
   ```

3. **Initialize a Git repository:**
   ```bash
   git init
   ```

4. **Add your GitHub repository as the remote:**
   ```bash
   # Replace YOUR_USERNAME with your actual GitHub username
   git remote add origin https://github.com/YOUR_USERNAME/PowerAI-Pitch-Deck.git
   
   # Example:
   # git remote add origin https://github.com/hlomohangcue/PowerAI-Pitch-Deck.git
   ```

5. **Add your pitch deck file:**
   ```bash
   git add index.html
   ```

6. **Commit your changes:**
   ```bash
   git commit -m "Initial pitch deck upload"
   ```

7. **Set the branch name and push to GitHub:**
   ```bash
   git branch -M main
   git push -u origin main
   ```

8. **Enter your GitHub credentials if prompted:**
   - Username: Your GitHub username
   - Password: Your GitHub personal access token ([Create one here](https://github.com/settings/tokens))

**Result:** Your pitch deck is now on GitHub! ✅

**Troubleshooting Command Line Issues:**
- **"git: command not found"** → Install Git from https://git-scm.com/downloads
- **Authentication failed** → Use a [Personal Access Token](https://github.com/settings/tokens) instead of your password
- **Permission denied** → Make sure you're the owner of the repository
- **Remote already exists** → Skip step 4 or use `git remote set-url origin URL`

---

### Step 4: Enable GitHub Pages (The Magic Step! ✨)

This is where you activate your website and make it live on the internet!

1. **Navigate to your repository:**
   - Go to `https://github.com/YOUR_USERNAME/PowerAI-Pitch-Deck`
   - Or click on your repository name from your GitHub homepage

2. **Open repository Settings:**
   - Look at the top menu bar of your repository
   - Click on the **⚙️ "Settings"** tab (rightmost tab)
   - ⚠️ **Not finding it?** Make sure you're logged in and on YOUR repository page

3. **Find GitHub Pages settings:**
   - In the left sidebar, scroll down until you find **"Pages"**
   - Click on **"Pages"**
   - You're now in the GitHub Pages configuration area

4. **Configure the source:**
   
   Under the **"Source"** section (also called "Build and deployment"):
   
   - **Source dropdown:** Select **"Deploy from a branch"**
   
   - **Branch dropdown:** 
     - Select **"main"** (or "master" if that's what you see)
     - This tells GitHub which branch to use for your website
   
   - **Folder dropdown:** 
     - Select **"/ (root)"**
     - This means your index.html is in the main folder
   
   - **Visual guide:**
     ```
     Source: Deploy from a branch
     Branch: [main ▼] [/ (root) ▼]
     ```

5. **Save your settings:**
   - Click the **"Save"** button
   - GitHub will show a message: "GitHub Pages source saved"

6. **Wait for deployment:**
   - GitHub Pages is now building your website!
   - **First-time deployment:** Takes 1-3 minutes
   - **Subsequent updates:** Usually 30-60 seconds
   - You'll see a message like: "Your site is ready to be published at..."
   - ⏳ **Be patient!** Refresh the page after 2 minutes

7. **Verify deployment:**
   - Refresh the Settings → Pages page
   - Look for a green success message:
     ```
     ✅ Your site is live at https://YOUR_USERNAME.github.io/PowerAI-Pitch-Deck/
     ```
   - If you see this - congratulations! Your deck is live! 🎉

**What if I don't see the green success message?**
- Wait another minute and refresh
- Check that your branch is set to "main" and folder is "/ (root)"
- Verify that index.html is in your repository root
- See Troubleshooting section below for more help

### Step 5: Access and Test Your Live Pitch Deck 🚀

Your pitch deck is now live on the internet! Let's verify it works.

**Your Pitch Deck URL:**
```
https://YOUR_USERNAME.github.io/PowerAI-Pitch-Deck/
```

**Real Example (adjust for your username):**
```
https://hlomohangcue.github.io/PowerAI-Pitch-Deck/
```

**Testing Your Deck:**

1. **Open your URL in a web browser:**
   - Copy your complete URL (including https://)
   - Paste it into a new browser tab
   - Press Enter

2. **What you should see:**
   - ✅ Your PowerAI pitch deck loads with the first slide
   - ✅ Professional green energy theme with PowerAI branding
   - ✅ Navigation arrows at the bottom
   - ✅ Smooth animations and transitions

3. **Test the navigation:**
   - Click the **right arrow** → to go to next slide
   - Click the **left arrow** ← to go back
   - Press **arrow keys** on keyboard (→ next, ← previous)
   - Press **Space bar** for next slide
   - On mobile: **Swipe left/right** to navigate

4. **Test all 12 slides:**
   - Navigate through all slides to ensure they all load
   - Check that text is readable
   - Verify images and content display correctly
   - Test any links (they should open in new tabs)

5. **Test on different devices:**
   - 💻 Desktop/laptop browser
   - 📱 Mobile phone (iOS/Android)
   - 📱 Tablet
   - Try different browsers (Chrome, Firefox, Safari, Edge)

**Troubleshooting Access Issues:**

❌ **"404 - Page not found"**
- Wait another 2-3 minutes (initial deployment takes time)
- Check your URL spelling (case-sensitive)
- Verify index.html is in repository root (not in a subfolder)
- Go back to Settings → Pages and confirm it says "Your site is live"

❌ **Blank page or doesn't load**
- Check browser console for errors (F12, then Console tab)
- Verify index.html uploaded completely
- Try incognito/private browsing mode (rules out cache issues)
- Try a different browser

❌ **Looks broken or styling is wrong**
- Hard refresh the page: Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)
- Check that the entire HTML file uploaded (not truncated)
- View page source (right-click → View Page Source) to verify content

✅ **Everything works perfectly?** → Proceed to Step 6!

---

### Step 6: Share Your Deck with the World 🌍

Now that your pitch deck is live, it's time to share it with investors and stakeholders!

**🔗 Ways to Share Your URL:**

1. **Direct Sharing:**
   - Copy your URL: `https://YOUR_USERNAME.github.io/PowerAI-Pitch-Deck/`
   - Share via email, SMS, messaging apps
   - Post on social media (LinkedIn, Twitter)

2. **Email Signature:**
   ```
   View PowerAI Pitch Deck: https://hlomohangcue.github.io/PowerAI-Pitch-Deck/
   ```

3. **LinkedIn Profile:**
   - Add to your "About" section
   - Include in posts about PowerAI
   - Share in relevant groups and with connections

4. **Business Cards:**
   - Add the URL to printed business cards
   - Create a QR code that links to your deck (use qr-code-generator.com)
   - Print QR code on cards for easy mobile access

5. **Investor Emails:**
   ```
   Subject: PowerAI - Renewable Energy Platform Investment Opportunity
   
   Dear [Investor Name],
   
   I'd like to introduce you to PowerAI, an AI-powered renewable energy 
   management platform for Africa.
   
   View our interactive pitch deck: 
   https://hlomohangcue.github.io/PowerAI-Pitch-Deck/
   
   I'd welcome the opportunity to discuss this further at your convenience.
   
   Best regards,
   [Your Name]
   ```

6. **During Presentations:**
   - Project the website during live pitches (instead of PowerPoint)
   - Share URL in virtual meeting chats (Zoom, Teams, Google Meet)
   - Include in slide decks as a reference link

**📊 Professional Tips:**

- ✅ Always test the link before sending
- ✅ Use link shorteners for cleaner URLs (bit.ly, tinyurl.com)
- ✅ Track link clicks with UTM parameters for analytics
- ✅ Create a memorable custom domain (optional - see below)
- ✅ Update the deck regularly to keep information current
- ✅ Have a PDF backup for offline presentations

**🎯 Strategic Sharing:**

- **Before meetings:** Send 24 hours in advance so investors can review
- **After meetings:** Include in thank-you follow-up emails
- **Pitch competitions:** Submit as supplementary material
- **Media inquiries:** Share with journalists covering your story
- **Partnership discussions:** Show potential partners your vision

---

### Step 7: Updating Your Pitch Deck (Maintaining Your Site) 🔄

Your pitch deck is live, but you'll want to update it over time. Here's how:

#### **Method A: Update via GitHub Web Interface (Easiest)**

1. **Go to your repository:**
   - Navigate to `https://github.com/YOUR_USERNAME/PowerAI-Pitch-Deck`

2. **Find and open index.html:**
   - Click on `index.html` in the file list
   - You'll see the file contents

3. **Edit the file:**
   - Click the **pencil icon** (✏️) in the top right ("Edit this file")
   - Make your changes directly in the web editor
   - Use Ctrl+F (Windows) or Cmd+F (Mac) to find specific text to change

4. **Commit (save) your changes:**
   - Scroll to bottom of page
   - Add a commit message describing your change:
     ```
     Update investor contact information
     ```
     or
     ```
     Add Q3 2024 traction metrics
     ```
   - Click **"Commit changes"**

5. **Wait for automatic deployment:**
   - GitHub Pages automatically rebuilds your site
   - Takes 30-60 seconds
   - Visit your live URL and hard-refresh (Ctrl+Shift+R) to see changes

#### **Method B: Update via Git Command Line**

If you used Git command line originally:

```bash
# Navigate to your pitch-deck folder
cd /path/to/PowerAI-Pitch-Deck/pitch-deck

# Make your changes to index.html (using any text editor)

# Check what changed
git status
git diff index.html

# Stage your changes
git add index.html

# Commit with a descriptive message
git commit -m "Update financial projections and add Q3 metrics"

# Push to GitHub
git push origin main

# Site will auto-update in 30-60 seconds
```

#### **What to Update Regularly:**

📅 **Monthly:**
- Traction metrics and user numbers
- Financial projections and revenue
- Partnership announcements
- Team updates (new hires)

📅 **Quarterly:**
- Market statistics and data
- Product features and roadmap progress
- Competitive landscape analysis
- Contact information (if changed)

📅 **Before Each Pitch:**
- Review all content for accuracy
- Update "last updated" date
- Test all links are working
- Verify contact information is current

---

### 🎓 Advanced GitHub Pages Features

#### **Custom Domain Setup (Optional)**

Make your pitch deck even more professional with a custom domain!

**Instead of:** `https://hlomohangcue.github.io/PowerAI-Pitch-Deck/`  
**Use:** `https://pitch.powerai.com` or `https://deck.powerai.co.ls`

**Steps:**

1. **Purchase a domain:**
   - Use domain registrars like Namecheap, GoDaddy, or Google Domains
   - Cost: ~$10-15/year
   - African domains (.co.za, .co.ls) available through AfriCC or local registrars

2. **Configure DNS:**
   - In your domain registrar's control panel
   - Add a CNAME record:
     ```
     Type: CNAME
     Host: pitch (or deck, or www)
     Value: YOUR_USERNAME.github.io
     TTL: 3600
     ```

3. **Add custom domain to GitHub:**
   - Go to Settings → Pages in your repository
   - Under "Custom domain", enter: `pitch.powerai.com`
   - Check "Enforce HTTPS"
   - Click Save

4. **Wait for DNS propagation:**
   - Takes 15 minutes to 48 hours
   - Check status at: https://www.whatsmydns.net/

**Result:** Your deck is now at your custom domain! 🎉

---

#### **Adding Google Analytics (Track Visitors)**

See how many investors view your deck and which slides they spend time on.

1. **Create Google Analytics account:**
   - Go to https://analytics.google.com/
   - Sign up (free) and create a property
   - Get your Measurement ID (looks like: G-XXXXXXXXXX)

2. **Add tracking code to your pitch deck:**
   - Edit index.html
   - Find the `</head>` tag (near line 200)
   - Add this code right BEFORE `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

3. **Replace G-XXXXXXXXXX with your actual Measurement ID**

4. **Commit and push changes**

5. **View analytics:**
   - Go to your Google Analytics dashboard
   - See real-time visitors, page views, and more
   - Track which slides get the most attention

**What you can learn:**
- How many investors viewed your deck
- Which slides they spent time on
- Geographic location of viewers
- What devices they used (mobile/desktop)
- How they found your deck (referral sources)

---

#### **Creating a QR Code for Easy Mobile Access**

Perfect for business cards and printed materials!

1. **Generate QR code:**
   - Go to https://www.qr-code-generator.com/ (free)
   - Select "URL" option
   - Paste your pitch deck URL
   - Customize design (optional):
     - Add PowerAI logo in center
     - Use green color scheme matching your brand
     - Add call-to-action text: "View Pitch Deck"

2. **Download QR code:**
   - High resolution (PNG or SVG)
   - Save for printing and digital use

3. **Use your QR code:**
   - Add to business cards
   - Include in printed marketing materials
   - Display at events and conferences
   - Add to presentation slides
   - Print on posters and banners

**Testing:** Scan with your phone's camera to verify it opens your deck!

---

### 🐛 Comprehensive Troubleshooting Guide

#### **Problem: GitHub Pages not showing my site**

**Symptoms:** Settings say "Your site is live" but URL shows 404 error

**Solutions:**
1. ✅ Wait 5 minutes - first deployment takes time
2. ✅ Check index.html is in repository ROOT (not in a subfolder)
3. ✅ Verify repository is PUBLIC (Settings → General → Visibility)
4. ✅ Confirm branch is set to "main" (Settings → Pages)
5. ✅ Try accessing: `https://YOUR_USERNAME.github.io/PowerAI-Pitch-Deck/index.html`
6. ✅ Check GitHub Status: https://www.githubstatus.com/
7. ✅ Disable browser extensions (especially ad blockers)
8. ✅ Try incognito/private browsing mode

---

#### **Problem: Changes not appearing on live site**

**Symptoms:** You updated index.html but website still shows old content

**Solutions:**
1. ✅ Wait 2-3 minutes for GitHub Pages to rebuild
2. ✅ Hard refresh browser: Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)
3. ✅ Clear browser cache and cookies
4. ✅ Check GitHub Actions tab - see if build is in progress or failed
5. ✅ Verify changes were committed (check repository file)
6. ✅ Try different browser or incognito mode
7. ✅ Check if you're editing the correct branch (should be "main")

---

#### **Problem: Styling looks broken or incomplete**

**Symptoms:** Pitch deck appears but colors, fonts, or layout is wrong

**Solutions:**
1. ✅ Hard refresh: Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)
2. ✅ Check browser console for errors:
   - Press F12 to open DevTools
   - Click "Console" tab
   - Look for red error messages
3. ✅ Verify complete HTML file uploaded (check file size matches original)
4. ✅ View page source (Right-click → View Page Source) - ensure CSS is present
5. ✅ Test in different browser (Chrome, Firefox, Safari)
6. ✅ Disable browser extensions temporarily
7. ✅ Check if you accidentally modified CSS in the `<style>` section

---

#### **Problem: Navigation not working (can't change slides)**

**Symptoms:** Stuck on first slide, arrows don't work, keyboard shortcuts fail

**Solutions:**
1. ✅ Ensure JavaScript is enabled in browser settings
2. ✅ Check browser console for JavaScript errors (F12 → Console)
3. ✅ Try different browser
4. ✅ Disable browser extensions (especially script blockers)
5. ✅ Verify the complete HTML file was uploaded (check `<script>` tags are present)
6. ✅ Test on different device
7. ✅ Clear cache and reload

---

#### **Problem: Mobile version not working properly**

**Symptoms:** Deck looks wrong on phone, swipe doesn't work, too small to read

**Solutions:**
1. ✅ Use actual mobile device for testing (not just browser resize)
2. ✅ Check viewport meta tag is present in HTML (it should be)
3. ✅ Try landscape orientation
4. ✅ Update to latest browser version
5. ✅ Clear mobile browser cache
6. ✅ Test on multiple mobile browsers (Chrome, Safari, Firefox)
7. ✅ Verify touch events aren't blocked by other scripts

---

#### **Problem: Can't upload to GitHub (authentication failed)**

**Symptoms:** Git push fails with "authentication failed" or "permission denied"

**Solutions:**
1. ✅ GitHub no longer accepts passwords - use Personal Access Token:
   - Go to https://github.com/settings/tokens
   - Click "Generate new token (classic)"
   - Give it a name: "PowerAI Pitch Deck Deploy"
   - Select scopes: Check "repo" (full control of private repositories)
   - Click "Generate token"
   - **Copy the token immediately** (you can't see it again!)
   - Use this token as your password when git asks
2. ✅ Configure Git credential helper to remember token:
   ```bash
   git config --global credential.helper store
   ```
3. ✅ Verify you're the repository owner
4. ✅ Check repository URL is correct:
   ```bash
   git remote -v
   ```
5. ✅ Try HTTPS URL instead of SSH:
   ```bash
   git remote set-url origin https://github.com/YOUR_USERNAME/PowerAI-Pitch-Deck.git
   ```

---

#### **Problem: Site is too slow to load**

**Symptoms:** Pitch deck takes long time to load or is unresponsive

**Solutions:**
1. ✅ Check your internet connection
2. ✅ GitHub Pages is fast - issue is likely local
3. ✅ Test from different location/network
4. ✅ Use online speed test: https://tools.pingdom.com/
5. ✅ Optimize images if you added any (use TinyPNG.com)
6. ✅ Check if your region has GitHub Pages restrictions
7. ✅ Consider using CDN for very large files

---

### 📊 Comparing GitHub Pages with Other Options

| Feature | GitHub Pages | Netlify | Vercel | Traditional Hosting |
|---------|--------------|---------|--------|-------------------|
| **Cost** | FREE forever | FREE (with limits) | FREE (with limits) | $5-50/month |
| **Setup Time** | 10 minutes | 5 minutes | 5 minutes | 30+ minutes |
| **Custom Domain** | ✅ Free | ✅ Free | ✅ Free | ✅ Usually included |
| **HTTPS/SSL** | ✅ Automatic | ✅ Automatic | ✅ Automatic | Extra cost/setup |
| **Version Control** | ✅ Built-in (Git) | ✅ Via GitHub | ✅ Via GitHub | ❌ Manual |
| **Deployment** | Git push | Git push or drag-drop | Git push or drag-drop | FTP/cPanel |
| **Best For** | Pitch decks, portfolios | Web apps | Web apps | Complex sites |
| **Learning Curve** | Moderate | Easy | Easy | High |

**Recommendation:** Stick with GitHub Pages for pitch decks - it's perfect for this use case!

---

### ✅ Complete Pre-Launch Checklist

Before sharing your deck with investors, verify:

**Content:**
- [ ] All 12 slides are present and display correctly
- [ ] Contact information is accurate and up-to-date
- [ ] Email addresses work and are monitored
- [ ] Phone numbers are current
- [ ] All statistics and metrics are current (within 3 months)
- [ ] No placeholder text remains (like "YOUR_EMAIL")
- [ ] Company name and branding are consistent
- [ ] Spelling and grammar checked

**Functionality:**
- [ ] All navigation works (arrows, keyboard, swipe)
- [ ] All 12 slides accessible
- [ ] No slides are blank or broken
- [ ] Smooth transitions between slides
- [ ] All links open and work correctly
- [ ] Demo app link works (if applicable)
- [ ] GitHub repository link works
- [ ] Site loads in under 3 seconds

**Cross-Platform Testing:**
- [ ] Tested on desktop (Windows/Mac/Linux)
- [ ] Tested on Chrome browser
- [ ] Tested on Firefox browser
- [ ] Tested on Safari browser (Mac/iPhone)
- [ ] Tested on mobile phone (actual device)
- [ ] Tested on tablet (if available)
- [ ] Landscape and portrait modes work on mobile
- [ ] Touch gestures work (swipe left/right)

**Professional Polish:**
- [ ] URL is professional and memorable
- [ ] QR code generated and tested
- [ ] PDF backup created (print to PDF)
- [ ] Analytics installed (optional but recommended)
- [ ] Custom domain configured (optional)
- [ ] Shared with team for feedback
- [ ] Practiced pitch using the deck
- [ ] Emergency contact method available

**Legal & Security:**
- [ ] No confidential information exposed publicly
- [ ] No customer data without permission
- [ ] Copyright/trademark compliance checked
- [ ] License information accurate (if applicable)
- [ ] Privacy policy link added (if collecting data)

**Documentation:**
- [ ] URL saved in safe place
- [ ] Login credentials documented
- [ ] Update process documented for team
- [ ] Backup files stored securely
- [ ] Version history maintained

---

### 🎯 Best Practices for Investor Presentations

**Before the Pitch:**
- ✅ Send deck URL 24 hours before meeting
- ✅ Test the site from different locations
- ✅ Have PDF backup ready
- ✅ Ensure all data is current
- ✅ Practice navigation thoroughly

**During the Pitch:**
- ✅ Use the live website (more impressive than PDF)
- ✅ Have backup device with deck loaded
- ✅ Test projector/screen before presentation
- ✅ Know keyboard shortcuts by heart
- ✅ Have printed one-pagers as handouts

**After the Pitch:**
- ✅ Email thank-you with deck URL
- ✅ Track if/when they view it (via analytics)
- ✅ Follow up within 48 hours
- ✅ Update deck with any new questions/answers
- ✅ Document feedback for improvements

**Ongoing Maintenance:**
- ✅ Update metrics monthly
- ✅ Refresh statistics quarterly
- ✅ Add new achievements immediately
- ✅ Keep contact information current
- ✅ Monitor analytics for engagement insights

---

### 📚 Additional Resources

**GitHub Pages Documentation:**
- Official Docs: https://docs.github.com/pages
- GitHub Pages Help: https://pages.github.com/
- GitHub Community: https://github.community/

**Learning Git & GitHub:**
- Git Tutorial: https://try.github.io/
- GitHub Skills: https://skills.github.com/
- Git Cheat Sheet: https://education.github.com/git-cheat-sheet-education.pdf

**Web Development Resources:**
- HTML Tutorial: https://www.w3schools.com/html/
- CSS Tutorial: https://www.w3schools.com/css/
- JavaScript Tutorial: https://www.w3schools.com/js/

**Tools & Services:**
- QR Code Generator: https://www.qr-code-generator.com/
- Link Shortener: https://bitly.com/
- Speed Test: https://tools.pingdom.com/
- DNS Checker: https://www.whatsmydns.net/
- Google Analytics: https://analytics.google.com/

---

### 🆘 Getting Help

**If you're stuck:**

1. **Check this guide again** - most issues are covered above
2. **Search GitHub Community** - https://github.community/
3. **Check GitHub Status** - https://www.githubstatus.com/
4. **Ask for help:**
   - GitHub Support (for GitHub Pages issues)
   - Stack Overflow (for HTML/CSS/JavaScript questions)
   - GitHub Discussions in this repository
   - Developer communities (Reddit r/webdev, r/github)

**When asking for help, include:**
- Your GitHub username (not password!)
- Repository name
- What you're trying to do
- What you expected to happen
- What actually happened
- Error messages (exact text)
- Screenshots (if applicable)
- Browser and OS you're using

---

### 🎉 Congratulations!

You've successfully deployed your PowerAI Pitch Deck to GitHub Pages!

**What you've accomplished:**
- ✅ Created a GitHub repository
- ✅ Deployed your pitch deck to the web
- ✅ Made it accessible 24/7 from anywhere
- ✅ Obtained a professional URL for investor communications
- ✅ Set up a system for easy updates
- ✅ Learned valuable Git and web deployment skills

**Your pitch deck is now:**
- 🌐 Live on the internet
- 📱 Mobile-friendly and responsive
- 🔒 Secure with HTTPS
- ⚡ Fast and reliable
- 💰 Completely FREE to host

**Next steps:**
- Share your deck with investors
- Monitor engagement with analytics
- Update content regularly
- Gather feedback and iterate
- Close that seed funding round! 💰

**Good luck with your PowerAI journey!** 🚀🌱

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
