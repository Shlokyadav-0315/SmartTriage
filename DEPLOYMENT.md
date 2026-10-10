# 🚀 GitHub Deployment Guide

Follow these simple steps to deploy your SmartTriage application to GitHub Pages.

## Prerequisites

- Git installed on your computer
- GitHub account created
- GitHub CLI (optional, but recommended)

---

## Step 1: Initialize Git Repository

Open your terminal/command prompt in the SmartTriage folder and run:

```bash
# Initialize git repository
git init

# Add all files
git add .

# Create initial commit
git commit -m "🎉 Initial commit: SmartTriage Healthcare App"
```

---

## Step 2: Create GitHub Repository

### Option A: Using GitHub Website (Easier)

1. Go to [github.com](https://github.com)
2. Click the **"+"** icon in top-right corner
3. Click **"New repository"**
4. Repository name: `SmartTriage`
5. Description: `AI-powered healthcare triage and clinic navigator`
6. Keep it **Public** (required for free GitHub Pages)
7. **DO NOT** initialize with README (we already have one)
8. Click **"Create repository"**

### Option B: Using GitHub CLI (Faster)

```bash
# Login to GitHub (first time only)
gh auth login

# Create repository
gh repo create SmartTriage --public --source=. --remote=origin --push
```

---

## Step 3: Push Your Code

If you used Option A above, run these commands (GitHub will show you these):

```bash
# Add GitHub as remote
git remote add origin https://github.com/YOUR-USERNAME/SmartTriage.git

# Rename branch to main (if needed)
git branch -M main

# Push code to GitHub
git push -u origin main
```

**Replace `YOUR-USERNAME` with your actual GitHub username!**

---

## Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **"Settings"** tab
3. Scroll down to **"Pages"** in the left sidebar
4. Under "Source", select:
   - Branch: **main**
   - Folder: **/ (root)**
5. Click **"Save"**
6. Wait 2-3 minutes for deployment

---

## Step 5: Get Your Live URL

After deployment completes, your app will be live at:

```
https://YOUR-USERNAME.github.io/SmartTriage/
```

**Example**: If your username is `johnsmith`, your URL will be:
```
https://johnsmith.github.io/SmartTriage/
```

---

## Step 6: Update README with Your URL

1. Open `README.md`
2. Find this line:
   ```markdown
   **👉 [Try SmartTriage Now](https://yourusername.github.io/SmartTriage) 👈**
   ```
3. Replace `yourusername` with your actual GitHub username
4. Find all other instances of `yourusername` and replace them
5. Save the file

```bash
# Commit the changes
git add README.md
git commit -m "📝 Update README with live demo URL"
git push
```

---

## 🎉 Success!

Your SmartTriage app is now live! Share your URL:

- **Live Demo**: `https://YOUR-USERNAME.github.io/SmartTriage/`
- **Repository**: `https://github.com/YOUR-USERNAME/SmartTriage`

---

## 🔄 Making Updates

Whenever you make changes to your code:

```bash
# Save your changes in the editor first, then:

git add .
git commit -m "✨ Your commit message here"
git push

# GitHub Pages will auto-update in 1-2 minutes
```

---

## 🐛 Troubleshooting

### Issue: GitHub Pages not working

**Solution 1**: Check if Pages is enabled
- Go to Settings → Pages
- Make sure "Branch: main" and "/ (root)" are selected

**Solution 2**: Wait a few minutes
- First deployment can take 5-10 minutes
- Check the "Actions" tab to see deployment progress

**Solution 3**: Check repository visibility
- Repository must be **Public** for free GitHub Pages
- Go to Settings → General → scroll to bottom
- Under "Danger Zone", you can change visibility

### Issue: 404 Page Not Found

**Solution**: Make sure your URL is correct
```
✅ Correct: https://username.github.io/SmartTriage/
❌ Wrong: https://username.github.io/SmartTriage/index.html
```

### Issue: Can't push to GitHub

**Solution 1**: Check authentication
```bash
# For HTTPS (recommended for beginners)
git remote set-url origin https://github.com/YOUR-USERNAME/SmartTriage.git

# Then enter your GitHub username and Personal Access Token (not password!)
```

**Solution 2**: Generate Personal Access Token
1. GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Generate new token (classic)
3. Give it "repo" permissions
4. Copy the token and use it as your password when pushing

---

## 📱 Share Your Project

Once deployed, share it on:

- LinkedIn: "🚀 Just deployed my healthcare app!"
- Twitter/X: "#HealthTech #AI #OpenSource"
- Dev.to: Write a blog post about your project
- Reddit: r/webdev, r/HealthIT
- Hackathon platforms: Include the live URL

---

## 🌟 Next Steps

1. ✅ Star your own repository (why not? 😄)
2. 🖼️ Add screenshots to README
3. 📹 Record a demo video
4. 🎨 Create a custom domain (optional)
5. 📊 Add Google Analytics (optional)

---

## 📞 Need Help?

- **Git Issues**: [Git Documentation](https://git-scm.com/doc)
- **GitHub Pages**: [GitHub Pages Docs](https://docs.github.com/en/pages)
- **General Help**: [GitHub Community](https://github.community/)

---

**Good luck with your hackathon! 🏆**
