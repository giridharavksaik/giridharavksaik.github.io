# Deployment Guide

This guide will help you deploy your React portfolio to the internet in minutes.

## 🚀 Quick Start (Recommended: Vercel)

### Step 1: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click **"New"** to create a new repository
3. Name it: `gitidhara-portfolio`
4. Click **"Create repository"**

### Step 2: Push Your Code to GitHub

```bash
cd /path/to/gitidhara-portfolio

# Initialize git (if not already done)
git init
git add .
git commit -m "Initial commit: Impressive React portfolio"

# Add remote repository
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/gitidhara-portfolio.git

# Push to GitHub
git push -u origin main
```

### Step 3: Deploy to Vercel

1. Go to [Vercel.com](https://vercel.com)
2. Click **"Sign Up"** and choose "Continue with GitHub"
3. Authorize Vercel to access your GitHub account
4. Click **"New Project"**
5. Select your `gitidhara-portfolio` repository
6. Click **"Import"**
7. Click **"Deploy"**

**Your portfolio is now live!** 🎉

Vercel will give you a URL like: `https://gitidhara-portfolio.vercel.app`

---

## 📋 Alternative Deployment Options

### Option 2: Netlify

1. **Build your project**
```bash
pnpm build
```

2. **Deploy to Netlify**
   - Go to [Netlify.com](https://netlify.com)
   - Sign in with GitHub
   - Click **"New site from Git"**
   - Select your repository
   - Click **"Deploy site"**

### Option 3: GitHub Pages

1. **Update vite.config.js**
```javascript
export default defineConfig({
  base: '/gitidhara-portfolio/', // Replace with your repo name
  plugins: [react()],
})
```

2. **Build the project**
```bash
pnpm build
```

3. **Deploy**
```bash
git add dist
git commit -m "Deploy to GitHub Pages"
git push
```

4. **Enable GitHub Pages**
   - Go to repository **Settings**
   - Scroll to **"Pages"**
   - Set source to `gh-pages` branch

---

## 🔐 Setting Up Web3Forms

### Step 1: Get Your Access Key

1. Go to [Web3Forms.com](https://web3forms.com)
2. Click **"Sign Up"** (free)
3. Create a new form
4. Copy your **Access Key**

### Step 2: Add to Your Portfolio

Edit `src/components/Contact.jsx` and replace:

```javascript
access_key: 'YOUR_WEB3FORMS_ACCESS_KEY', // Replace this with your actual key
```

With your actual Web3Forms access key.

### Step 3: Test the Form

1. Go to your live portfolio
2. Scroll to "Get In Touch"
3. Fill out the contact form
4. Click "Send Message"
5. Check your email for the message

---

## 🌐 Custom Domain (Optional)

### Using Vercel

1. Go to your Vercel project settings
2. Click **"Domains"**
3. Click **"Add"**
4. Enter your domain name
5. Follow the instructions to update your DNS settings

### Using Netlify

1. Go to your Netlify site settings
2. Click **"Domain management"**
3. Click **"Add custom domain"**
4. Enter your domain name
5. Follow the instructions to update your DNS settings

---

## 🔄 Continuous Deployment

Both Vercel and Netlify support automatic deployments:

- **Push to GitHub** → **Automatic deployment** → **Live update**

No manual deployment needed! Just push your changes and they'll be live in seconds.

---

## 📊 Monitoring & Analytics

### Vercel Analytics
- Go to your Vercel dashboard
- View real-time analytics
- Monitor performance metrics

### Netlify Analytics
- Go to your Netlify site settings
- Enable analytics
- View traffic and performance data

---

## 🐛 Troubleshooting

### Build Fails on Vercel

**Solution**: Make sure all dependencies are installed
```bash
pnpm install
```

### Contact Form Not Working

**Solution**: Check your Web3Forms access key is correct in `Contact.jsx`

### Website Shows 404

**Solution**: Make sure you've pushed to GitHub and the deployment completed

---

## 📝 Environment Variables (Optional)

If you need to keep sensitive data secret:

1. Create a `.env.local` file:
```
VITE_WEB3FORMS_KEY=your_access_key_here
```

2. Update `Contact.jsx`:
```javascript
access_key: import.meta.env.VITE_WEB3FORMS_KEY,
```

3. Add `.env.local` to `.gitignore`

4. In Vercel/Netlify settings, add the environment variable

---

## ✅ Deployment Checklist

- [ ] GitHub repository created
- [ ] Code pushed to GitHub
- [ ] Vercel/Netlify project created
- [ ] Website is live
- [ ] Web3Forms access key added
- [ ] Contact form tested
- [ ] Custom domain configured (optional)
- [ ] Analytics enabled (optional)

---

## 🎉 You're Done!

Your impressive React portfolio is now live on the internet!

**Share your portfolio with:**
- Recruiters
- Potential clients
- Friends and family
- On your resume
- On LinkedIn

Good luck! 🚀
