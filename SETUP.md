# 🚀 Portfolio Setup Guide

Welcome! This is a **fully customizable, open-source Data Analyst portfolio template**. Follow this guide to clone, customize, and deploy your own version.

---

## 📋 Table of Contents

1. [Quick Start](#quick-start)
2. [Customization Guide](#customization-guide)
3. [File-by-File Instructions](#file-by-file-instructions)
4. [Local Testing](#local-testing)
5. [GitHub Pages Deployment](#github-pages-deployment)
6. [Advanced Customization](#advanced-customization)
7. [Troubleshooting](#troubleshooting)

---

## ⚡ Quick Start

### Step 1: Clone the Repository

```bash
git clone https://github.com/VikasDs007/VikasDs007.github.io.git my-portfolio
cd my-portfolio
```

Or **use this as a template** on GitHub:
- Go to [VikasDs007.github.io](https://github.com/VikasDs007/VikasDs007.github.io)
- Click **"Use this template"** → **"Create a new repository"**
- Name it `your-username.github.io` (important for GitHub Pages)

### Step 2: Update Core Information

Replace these placeholders throughout the project:

| Item | Find & Replace | Files |
|------|--------|-------|
| **Name** | `Vikas Chaurasia` | `index.html`, `README.md`, `manifest.json` |
| **Title** | `Data Analyst` | `index.html`, `README.md` |
| **Email** | `vikasjchaurasia@gmail.com` | `index.html` |
| **Phone** | `+91 9987056798` | `index.html` |
| **Location** | `Mumbai, India` | `index.html`, `README.md` |
| **GitHub Username** | `VikasDs007` | `index.html`, `README.md` |
| **LinkedIn Profile** | `vikasds007` | `index.html`, `README.md` |

### Step 3: Replace Project Information

Edit the **3 featured projects** in `index.html`:
- Project title, description, impact metrics
- GitHub repository links
- Dashboard images

### Step 4: Test Locally

```bash
cd my-portfolio
python3 -m http.server 8080 --bind 127.0.0.1
# Open browser → http://localhost:8080
```

### Step 5: Deploy to GitHub Pages

```bash
git add .
git commit -m "Customize portfolio with personal info"
git push origin main
```

✅ Your portfolio will be live at: `https://your-username.github.io`

---

## 📝 Customization Guide

### 1. Personal Information

**File: `index.html` (Lines 1-50)**

```html
<!-- Update these meta tags -->
<meta name="description" content="YOUR NAME - YOUR TITLE specializing in YOUR SKILLS">
<meta property="og:title" content="YOUR NAME - YOUR TITLE">
<meta property="og:description" content="Your portfolio description here">
```

**File: `manifest.json`**

```json
{
  "name": "Your Name - Your Title Portfolio",
  "short_name": "Your Name",
  "description": "Your portfolio description"
}
```

---

### 2. Contact Information

**File: `index.html` (Search for "Contact Section")**

Find these sections and update:

```html
<!-- Email -->
<p class="text-gray-300 text-xs">your-email@gmail.com</p>

<!-- Phone -->
<p class="text-gray-300 text-sm">+91 YOUR-PHONE</p>

<!-- Location -->
<p class="text-gray-300 text-sm">Your City, Country</p>

<!-- LinkedIn & GitHub Links -->
<a href="https://www.linkedin.com/in/your-username/">LinkedIn</a>
<a href="https://github.com/your-username">GitHub</a>

<!-- Resume Download -->
<a href="assets/docs/Your_Name_Resume.pdf" download>Resume</a>
```

---

### 3. Hero Section

**File: `index.html` (Search for "Hero Section")**

```html
<h1 class="text-5xl md:text-7xl font-bold mb-4">
    Your Name Here
</h1>
<p class="text-xl md:text-2xl text-gray-400 font-mono">
    Your Title | Your Specialty | Your Focus
</p>

<!-- Update Stats Cards -->
<div class="text-lg md:text-xl font-bold">Your Degree</div>
<div class="text-xs md:text-sm text-gray-400">Your Field &</div>
<div class="text-xs text-neon-blue mt-1">Your Specialization</div>
```

---

### 4. About Section

**File: `index.html` (Search for "About Section")**

```html
<h3 class="text-2xl font-bold text-white">Your Name</h3>
<p class="text-gray-400 text-sm font-mono">Your Professional Title</p>

<!-- Update About narrative -->
<p class="text-gray-300 mb-4 text-sm leading-relaxed">
    Write your professional background here. Focus on:
    - Your core competencies
    - Years of experience
    - Key achievements
    - Technology expertise
</p>

<!-- Update Skills Section -->
<!-- Replace skill tags with your skills -->
```

---

### 5. Featured Projects

**File: `index.html` (Search for "Project 1", "Project 2", "Project 3")**

For each project, update:

```html
<!-- Project Title -->
<h3 class="text-xl font-bold text-white">
    Your Project Title
</h3>

<!-- Project Description -->
<p class="text-gray-300 mb-4 text-sm leading-relaxed">
    Project description: what problem it solves, tools used, outcomes achieved.
</p>

<!-- Impact Metrics -->
<div class="text-xs font-mono">
    Impact: X datasets analyzed, Y% improvement, Z records processed
</div>

<!-- Tech Tags -->
<span class="px-2 py-1 bg-neon-blue/20">Your Tech 1</span>
<span class="px-2 py-1 bg-neon-purple/20">Your Tech 2</span>

<!-- GitHub Links -->
<a href="https://github.com/your-username/your-project">View Project</a>
```

---

### 6. Dashboard Images

**File: `index.html` & `assets/images/dashboards/`**

Replace dashboard images:

```bash
# Move your dashboard screenshots to:
assets/images/dashboards/

# Update image references in index.html:
<img src="assets/images/dashboards/YOUR_IMAGE.png" alt="Your Dashboard">
```

**Recommended Image Specifications:**
- Format: PNG or JPG
- Size: 800x600px or wider (landscape)
- Compression: Optimize before uploading (reduce file size)

---

### 7. Resume & Documents

**Files: `assets/docs/`**

1. Replace resume:
   ```bash
   cp your_resume.pdf assets/docs/Your_Name_Resume.pdf
   ```

2. Update download link in `index.html`:
   ```html
   <a href="assets/docs/Your_Name_Resume.pdf" download>
   ```

3. Update in README.md:
   ```markdown
   **Resume:** [Download PDF](./assets/docs/Your_Name_Resume.pdf)
   ```

---

### 8. Profile Picture

**File: `assets/images/Vikas.png`**

Replace with your profile picture:

```bash
# Remove old image
rm assets/images/Vikas.png

# Add your image (rename to match reference in index.html)
cp your-photo.png assets/images/your-name.png
```

Update reference in `index.html`:
```html
<img src="assets/images/your-name.png" alt="Your Name">
```

---

## 🔍 File-by-File Instructions

### `index.html` (Main Portfolio)

**Lines to Update:**

| Section | Lines | What to Change |
|---------|-------|-----------------|
| Meta tags (SEO) | 1-30 | Name, title, keywords, description |
| Hero section | 730-850 | Name, tagline, stats cards |
| About section | 850-1000 | Bio, title, skills narrative |
| Projects | 1090-1400 | 3 project details + GitHub links |
| Contact info | 1410-1450 | Email, phone, location, social links |
| Skills section | Search "Skills" | Add/remove your tech skills |

### `README.md`

Replace:
- `Vikas Chaurasia` → Your Name
- `Data Analyst` → Your Title/Role
- Project descriptions with your projects
- LinkedIn/GitHub URLs
- "Last Updated" date

### `manifest.json`

```json
{
  "name": "Your Name - Your Title Portfolio",
  "short_name": "Your Name",
  "description": "Your professional bio/summary",
  "background_color": "#0F0F23",
  "theme_color": "#00D4FF"
}
```

---

## 💻 Local Testing

### Prerequisites

- Python 3.8+ installed
- Web browser (Chrome, Firefox, Safari, Edge)
- Git installed

### Running Locally

**Option 1: Using Python HTTP Server (Recommended)**

```bash
cd my-portfolio
python3 -m http.server 8080 --bind 127.0.0.1
```

Then open: **http://localhost:8080**

**Option 2: Using Python Virtual Environment**

```bash
cd my-portfolio
python3 -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
python3 -m http.server 8080
```

**Option 3: Using Node.js (if installed)**

```bash
# Install simple HTTP server
npm install -g http-server

# Run
http-server .
```

### Testing Checklist

- [ ] All links work (GitHub, LinkedIn, resume download)
- [ ] Images load correctly (dashboards, profile pic)
- [ ] Form submission works
- [ ] Mobile responsiveness (test on phone/tablet)
- [ ] Dark theme displays correctly
- [ ] Animations smooth on scroll
- [ ] No console errors (F12 → Console)

---

## 🚀 GitHub Pages Deployment

### Prerequisites

You need a GitHub account and this repository forked/cloned.

### Step 1: Create Repository

Create a new repository named: **`your-username.github.io`**

(This is critical! GitHub Pages recognizes this naming convention)

### Step 2: Push Your Changes

```bash
# Navigate to your portfolio folder
cd my-portfolio

# Initialize Git (if not already cloned)
git init
git add .
git commit -m "Initial portfolio setup with personal info"

# Add remote
git remote add origin https://github.com/YOUR-USERNAME/YOUR-USERNAME.github.io.git

# Push to main branch
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages**
3. Under "Build and deployment":
   - Source: **Deploy from a branch**
   - Branch: **main** (or master)
   - Folder: **/ (root)**
4. Click **Save**

### Step 4: Verify Deployment

Wait 1-2 minutes, then visit: **https://your-username.github.io**

✅ Your portfolio is now live!

---

## 🎨 Advanced Customization

### Change Color Theme

**File: `index.html` (Search for color definitions)**

Default neon colors:
- Blue: `#00D4FF`
- Purple: `#8B5CF6`
- Green: `#00FF88`

To change globally, replace in `<style>`:

```css
.neon-blue: '#YOUR-COLOR';
.neon-purple: '#YOUR-COLOR';
.neon-green: '#YOUR-COLOR';
```

### Modify Fonts

**File: `index.html` (Line ~118)**

```html
<link href="https://fonts.googleapis.com/css2?family=YOUR-FONT:wght@400;700&display=swap" rel="stylesheet">
```

Then update Tailwind config:
```javascript
fontFamily: {
    'mono': ['YOUR-FONT', 'monospace'],
}
```

### Add Analytics

**Google Analytics:**

1. Create account at [google.com/analytics](https://google.com/analytics)
2. Get your Tracking ID (format: G-XXXXXXXXXX)
3. Find this line in `index.html`:
   ```html
   gtag('config', 'G-YOUR-ID');
   ```
4. Replace with your ID

### Add Contact Form Functionality

Current form uses EmailJS. To enable:

1. Sign up at [emailjs.com](https://www.emailjs.com/)
2. Get your Service ID, Template ID, and Public Key
3. Find this section in `index.html`:
   ```javascript
   emailjs.init("YOUR-PUBLIC-KEY");
   ```
4. Replace with your keys

---

## 🛠️ Troubleshooting

### **Issue: Images not loading locally**

**Solution:**
- Use absolute paths from root: `/assets/images/dashboards/image.png`
- Or run HTTP server instead of opening file directly

### **Issue: Links not working**

**Solution:**
- Check URL format: Must be full URLs for external links
- Use relative paths for internal files: `assets/docs/resume.pdf`

### **Issue: Form not sending emails**

**Solution:**
- Make sure you've set up EmailJS credentials
- Check browser console (F12) for error messages
- Test on production (localhost might have restrictions)

### **Issue: Portfolio not live on GitHub Pages**

**Solution:**
1. Repository name must be `your-username.github.io`
2. Verify settings → Pages → shows "Your site is live at..."
3. Wait 2-5 minutes for first deployment
4. Clear browser cache or use incognito window
5. Check for any build errors in GitHub Actions tab

### **Issue: Animations not working**

**Solution:**
- Ensure JavaScript is enabled
- Clear browser cache (Ctrl+Shift+Delete / Cmd+Shift+Delete)
- Test in different browser
- Check console for JS errors

### **Issue: Mobile layout looks wrong**

**Solution:**
- Hard refresh: Ctrl+F5 (Windows) / Cmd+Shift+R (Mac)
- Check viewport meta tag in `<head>`
- Test in actual mobile device, not just browser DevTools

---

## 📚 Additional Resources

- **Tailwind CSS Docs**: [tailwindcss.com](https://tailwindcss.com)
- **GitHub Pages Docs**: [pages.github.com](https://pages.github.com)
- **Web Design Best Practices**: [web.dev](https://web.dev)
- **SEO Optimization**: [moz.com/beginners-guide-to-seo](https://moz.com/beginners-guide-to-seo)

---

## 🤝 Contributing Back

Made improvements? Share them!

1. Fork the original repository
2. Create a feature branch: `git checkout -b feature/improvement`
3. Commit changes: `git commit -m "Add feature"`
4. Push: `git push origin feature/improvement`
5. Open a Pull Request

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

## 📄 License

This portfolio template is **MIT Licensed** - free to use, modify, and distribute. See [LICENSE.md](LICENSE.md) for details.

---

## 🎉 You're All Set!

Your portfolio is ready to showcase your skills to the world. 

**Next Steps:**
1. Customize all personal information
2. Test locally
3. Deploy to GitHub Pages
4. Share on LinkedIn, Twitter, and your resume
5. Keep projects & skills updated

Good luck! 🚀
