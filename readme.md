# Portfolio Website - GitHub Pages Setup Guide

This is your personal portfolio website, optimized for easy editing and GitHub Pages hosting.

## 📁 File Structure

Your portfolio consists of these files:
```
your-portfolio/
├── index.html              # Main HTML file (don't edit directly)
├── style.css              # All styling (customize colors/fonts here)
├── script.js              # JavaScript functionality
├── portfolio-config.json  # **EDIT THIS FILE** to update content
└── README.md             # This guide
```

## ✏️ How to Edit Your Portfolio

### Easy Way: Edit Content Only
**Simply edit `portfolio-config.json`** to update:
- Personal information (name, email, phone, LinkedIn)
- About section text
- Work experience
- Skills and technologies
- Statistics
- Location cards

### Advanced: Customize Design
Edit `style.css` to change:
- Colors (search for `--primary`, `--secondary`, `--accent`)
- Fonts
- Spacing and layout
- Animations

## 🚀 Host on GitHub Pages (Free!)

### Step 1: Create a GitHub Account
1. Go to [github.com](https://github.com)
2. Click "Sign up" and create your account

### Step 2: Create a New Repository
1. Click the "+" icon in the top-right corner
2. Select "New repository"
3. Name it: `your-username.github.io` (replace with your actual GitHub username)
   - Example: If your username is `ashishdubey`, name it `ashishdubey.github.io`
4. Make it **Public**
5. Click "Create repository"

### Step 3: Upload Your Files

#### Option A: Using GitHub Website (Easiest)
1. In your new repository, click "uploading an existing file"
2. Drag and drop all 5 files:
   - index.html
   - style.css
   - script.js
   - portfolio-config.json
   - README.md
3. Scroll down and click "Commit changes"

#### Option B: Using GitHub Desktop (Recommended)
1. Download [GitHub Desktop](https://desktop.github.com/)
2. Install and sign in
3. Click "Clone repository" → Select your portfolio repo
4. Choose a local folder
5. Copy all your portfolio files into that folder
6. Open GitHub Desktop
7. Write a commit message: "Initial portfolio upload"
8. Click "Commit to main"
9. Click "Push origin"

#### Option C: Using Git Command Line
```bash
# Navigate to your portfolio folder
cd path/to/your-portfolio

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial portfolio upload"

# Add your GitHub repository
git remote add origin https://github.com/your-username/your-username.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 4: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click "Settings"
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select:
   - Branch: **main**
   - Folder: **/ (root)**
5. Click "Save"

### Step 5: Access Your Website
After 2-3 minutes, your website will be live at:
```
https://your-username.github.io
```

Example: `https://ashishdubey.github.io`

## 🔄 Updating Your Portfolio

### Method 1: GitHub Website
1. Go to your repository on GitHub
2. Click on `portfolio-config.json`
3. Click the pencil icon (✏️) to edit
4. Make your changes
5. Scroll down and click "Commit changes"
6. Wait 1-2 minutes for changes to appear on your website

### Method 2: GitHub Desktop
1. Open the local folder with your files
2. Edit `portfolio-config.json` in any text editor
3. Save your changes
4. Open GitHub Desktop
5. Write a commit message: "Updated portfolio content"
6. Click "Commit to main"
7. Click "Push origin"
8. Wait 1-2 minutes for changes to go live

## 📝 Editing Guide

### Change Your Name and Contact Info
```json
"personal": {
  "name": "Your Name",
  "email": "your.email@example.com",
  "phone": "+1 (xxx) xxx-xxxx",
  "linkedin": "https://linkedin.com/in/yourprofile"
}
```

### Add or Remove Work Experience
```json
"experience": [
  {
    "logo": "H",
    "title": "Your Job Title",
    "company": "Company Name",
    "location": "City, Country",
    "duration": "Start Date - End Date",
    "description": "What you did in this role...",
    "achievements": ["Achievement 1", "Achievement 2"]
  }
]
```

### Update Skills
```json
"skills": [
  {
    "icon": "💻",
    "title": "Category Name",
    "tags": ["Skill 1", "Skill 2", "Skill 3"]
  }
]
```

## 🎨 Customization Tips

### Change Color Scheme
Edit `style.css` and find these lines:
```css
:root {
    --primary: #4b2e83;    /* Main purple color */
    --secondary: #b7a57a;  /* Gold color */
    --accent: #00c9ff;     /* Bright blue */
    --dark: #0a0a0a;       /* Background */
    --light: #f5f5f5;      /* Light sections */
}
```

### Use Your Own Images
Replace the Unsplash URLs in:
- `index.html` (hero background)
- `portfolio-config.json` (location cards)

## ❓ Troubleshooting

### Website Not Loading?
1. Wait 3-5 minutes after pushing changes
2. Check GitHub Pages is enabled in Settings → Pages
3. Make sure repository is named `your-username.github.io`
4. Clear your browser cache (Ctrl+Shift+R or Cmd+Shift+R)

### Content Not Showing?
1. Check `portfolio-config.json` for JSON syntax errors
2. Use [JSONLint](https://jsonlint.com/) to validate your JSON
3. Check browser console (F12) for errors

### Changes Not Appearing?
1. Wait 1-2 minutes after pushing
2. Hard refresh your browser (Ctrl+Shift+R or Cmd+Shift+R)
3. Check that you committed and pushed your changes

## 🆘 Need Help?

- **JSON Validation**: [jsonlint.com](https://jsonlint.com/)
- **GitHub Pages Guide**: [pages.github.com](https://pages.github.com/)
- **GitHub Support**: [support.github.com](https://support.github.com/)

## 📱 Custom Domain (Optional)

Want to use your own domain (like `yourname.com`)?

1. Buy a domain from [Namecheap](https://namecheap.com) or [Google Domains](https://domains.google)
2. In your repository, create a file named `CNAME`
3. Add your domain name: `yourname.com`
4. In your domain registrar, add these DNS records:
   ```
   A Record: 185.199.108.153
   A Record: 185.199.109.153
   A Record: 185.199.110.153
   A Record: 185.199.111.153
   ```
5. Wait 24-48 hours for DNS propagation

---

## 🎉 You're All Set!

Your portfolio is now live and easily editable. Just update `portfolio-config.json` whenever you want to make changes!

**Live Site**: `https://your-username.github.io`

Remember to update your portfolio regularly with new projects and experiences! 🚀