# 🚀 GitHub Deployment Guide
## How to Publish This Presentation as a Live Website

---

## 📋 Prerequisites
- A GitHub account (free at github.com)
- Git installed on your computer (or use GitHub.com directly)

---

## 🗂️ Repository File Structure

```
egypt-economic-2024/              ← Your repository root
├── README.md                     ← Main overview page (renders on GitHub)
├── _config.yml                   ← GitHub Pages configuration
├── .github/
│   └── workflows/
│       └── deploy.yml            ← Auto-deploy workflow
└── docs/
    ├── index.html                ← 🌐 Live visual website (GitHub Pages)
    ├── timeline.md               ← Detailed chronological timeline
    ├── investments.md            ← Major deals deep-dive
    ├── regional.md               ← MENA comparison analysis
    └── resources.md              ← Data sources & references
```

---

## Step 1 — Create GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Repository name: `egypt-economic-2024`
3. Set to **Public** (required for free GitHub Pages)
4. Do **not** initialize with README (you'll upload yours)
5. Click **Create repository**

---

## Step 2 — Upload Files

### Option A: GitHub Web Interface (Easiest)
1. On your new empty repo page, click **"uploading an existing file"**
2. Drag and drop ALL files maintaining the folder structure:
   - `README.md` → root
   - `_config.yml` → root
   - `.github/workflows/deploy.yml` → create folders
   - `docs/index.html` → docs folder
   - `docs/timeline.md` → docs folder
   - `docs/investments.md` → docs folder
   - `docs/regional.md` → docs folder
   - `docs/resources.md` → docs folder
3. Commit with message: `"Initial commit: Egypt Economic Landscape 2024"`

### Option B: Git Command Line
```bash
cd egypt-economic-2024
git init
git add .
git commit -m "Initial commit: Egypt Economic Landscape 2024"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/egypt-economic-2024.git
git push -u origin main
```

---

## Step 3 — Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** tab
3. Click **Pages** in the left sidebar
4. Under **Source**, select: **"GitHub Actions"**
5. The `deploy.yml` workflow will auto-trigger on your next push

---

## Step 4 — Wait for Deployment (~2 minutes)

1. Go to **Actions** tab in your repository
2. Watch the "Deploy Egypt Economic Presentation to GitHub Pages" workflow run
3. Green ✅ = deployed successfully

---

## Step 5 — Access Your Live Site

Your site will be live at:
```
https://YOUR_USERNAME.github.io/egypt-economic-2024/
```

The README.md renders automatically on the GitHub repo page.

---

## 📌 Key URLs After Deployment

| Page | URL |
|------|-----|
| 🌐 Visual Website | `https://YOUR_USERNAME.github.io/egypt-economic-2024/` |
| 📋 GitHub README | `https://github.com/YOUR_USERNAME/egypt-economic-2024` |
| 📅 Timeline | Click link in README |
| 💰 Investments | Click link in README |
| 🌍 Regional | Click link in README |
| 📚 Resources | Click link in README |

---

## 🔄 Updating Content

Any push to `main` branch automatically redeploys via GitHub Actions.

To update a file:
1. Navigate to the file on GitHub.com
2. Click the ✏️ pencil (edit) icon
3. Make changes
4. Commit → deployment triggers automatically

---

## ✅ Checklist

- [ ] Repository created as Public
- [ ] All files uploaded with correct folder structure
- [ ] GitHub Pages enabled (Source: GitHub Actions)
- [ ] First workflow run completed successfully
- [ ] Live URL tested and working
- [ ] README renders correctly on GitHub repo page
- [ ] All internal links working (timeline, investments, regional, resources)

---

*Questions? Open an Issue on your GitHub repository.*
