# 🚀 Giridhara Portfolio - Quick Start Guide

## 📥 Step 1: Download & Extract Files

### Option A: ZIP File (Recommended for Windows)
1. Download: `gitidhara-portfolio.zip`
2. Right-click → Extract All
3. Open the extracted `gitidhara-portfolio` folder

### Option B: TAR.GZ File (For Mac/Linux)
1. Download: `gitidhara-portfolio.tar.gz`
2. Run: `tar -xzf gitidhara-portfolio.tar.gz`
3. Open the extracted `gitidhara-portfolio` folder

---

## 💻 Step 2: Setup on Your Computer

### Requirements
- **Node.js** 16+ (Download from https://nodejs.org)
- **Git** (Download from https://git-scm.com)

### Install Dependencies
```bash
cd gitidhara-portfolio
npm install
# or if you have pnpm:
pnpm install
```

### Run Locally
```bash
npm run dev
# or
pnpm dev
```

Your portfolio will open at: `http://localhost:5173`

---

## 📤 Step 3: Upload to GitHub

### Create GitHub Repository
1. Go to https://github.com/new
2. Repository name: `gitidhara-portfolio`
3. Click "Create repository"

### Push Your Code
```bash
cd gitidhara-portfolio

# Initialize git
git init
git add .
git commit -m "Initial commit: Impressive React portfolio"

# Add remote
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/gitidhara-portfolio.git

# Push to GitHub
git push -u origin main
```

---

## 🌐 Step 4: Deploy to Vercel (Permanent Website)

### Deploy
1. Go to https://vercel.com
2. Click "New Project"
3. Select your GitHub repository
4. Click "Deploy"

**Your portfolio is now live!** 🎉

Your URL will be: `https://gitidhara-portfolio.vercel.app`

---

## ✅ Checklist

- [ ] Downloaded and extracted files
- [ ] Installed Node.js
- [ ] Ran `npm install`
- [ ] Tested locally with `npm run dev`
- [ ] Created GitHub account
- [ ] Pushed code to GitHub
- [ ] Deployed to Vercel
- [ ] Portfolio is live!

---

## 📝 Important Files

| File | Purpose |
|------|---------|
| `README.md` | Full documentation |
| `DEPLOYMENT.md` | Detailed deployment guide |
| `package.json` | Project dependencies |
| `src/` | React components |
| `.gitignore` | Files to ignore in Git |

---

## 🔧 Customization

Before deploying, update:
- `src/components/Contact.jsx` - Your email is already set to giridharak2301@gmail.com
- `src/components/Hero.jsx` - Your name and bio
- `src/components/Projects.jsx` - Your projects
- `src/components/Experience.jsx` - Your work experience
- `src/components/Certifications.jsx` - Your certifications
- `src/components/Achievements.jsx` - Your achievements

---

## 🆘 Troubleshooting

### "npm: command not found"
→ Install Node.js from https://nodejs.org

### "Port 5173 is in use"
→ Run: `npm run dev -- --port 3000`

### Build fails
→ Run: `npm install` again

### Git not working
→ Install Git from https://git-scm.com

---

## 📞 Support

- **Node.js Issues**: https://nodejs.org/docs
- **Git Help**: https://git-scm.com/doc
- **React Docs**: https://react.dev
- **Vercel Docs**: https://vercel.com/docs

---

## 🎉 You're All Set!

Your impressive React portfolio is ready to go live. Follow the steps above and you'll have a permanent website in minutes!

Good luck! 🚀
