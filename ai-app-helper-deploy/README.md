# AI App Design Helper - Deployment Guide

A comprehensive AI-powered tool for designing and building apps, featuring six connected agents.

---

## 🚀 Deploy to Vercel (Free)

### Step 1: Create a GitHub Account (if you don't have one)

1. Go to **https://github.com**
2. Click **"Sign up"**
3. Follow the steps to create your account

---

### Step 2: Create a New Repository

1. Log in to GitHub
2. Click the **"+"** button in the top right corner
3. Select **"New repository"**
4. Name it `ai-app-helper` (or any name you like)
5. Keep it **Public** (free) or **Private** (also free)
6. **DO NOT** check "Add a README file"
7. Click **"Create repository"**

---

### Step 3: Upload the Files

After creating the repository, you'll see a page with setup instructions. 

**Easy method (using the website):**

1. On your new repository page, click **"uploading an existing file"**
2. Drag and drop ALL the files and folders from this project:
   - `api/` folder (contains `messages.js`)
   - `public/` folder (contains `index.html`)
   - `package.json`
   - `vercel.json`
   - `.gitignore`
3. Click **"Commit changes"**

**Important:** Make sure the folder structure stays the same:
```
ai-app-helper/
├── api/
│   └── messages.js
├── public/
│   └── index.html
├── package.json
├── vercel.json
└── .gitignore
```

---

### Step 4: Create a Vercel Account

1. Go to **https://vercel.com**
2. Click **"Sign Up"**
3. Select **"Continue with GitHub"**
4. Authorize Vercel to access your GitHub account

---

### Step 5: Deploy Your App

1. Once logged into Vercel, click **"Add New..."** → **"Project"**
2. Find your `ai-app-helper` repository in the list
3. Click **"Import"**
4. Keep all the default settings
5. Click **"Deploy"**
6. Wait 1-2 minutes for deployment to complete

---

### Step 6: Get Your Live URL

Once deployed, Vercel will give you a URL like:
```
https://ai-app-helper-yourname.vercel.app
```

**That's it!** Share this URL with anyone and they can use the app.

---

## 📝 How Users Use the App

When someone visits your URL:

1. Click **"Sign In"** (demo mode, no password needed)
2. Go to **Settings**
3. Add their own Anthropic API key
4. Start creating projects!

**Each user needs their own API key** from https://console.anthropic.com

---

## 🔄 Making Updates

If you want to change the app later:

1. Go to your GitHub repository
2. Edit the files you want to change
3. Vercel will automatically redeploy within minutes

---

## ❓ Troubleshooting

### "Failed to fetch" or API errors
- Make sure the `api/messages.js` file is in the `api/` folder
- Check that Vercel deployed successfully (no build errors)

### Page not loading
- Make sure `index.html` is inside the `public/` folder
- Check the Vercel deployment logs for errors

### Can't find repository in Vercel
- Make sure you authorized Vercel to access your GitHub
- Try clicking "Adjust GitHub App Permissions" in Vercel

---

## 🔐 Security Notes

- API keys are stored in each user's browser only
- Keys are never stored on the server
- Each user is responsible for their own API usage and billing

---

## 💡 Tips

- Bookmark your Vercel dashboard to check deployment status
- You can add a custom domain in Vercel settings (optional)
- The free tier of Vercel is very generous for this type of app

---

## Need Help?

If you get stuck, the most common issues are:
1. Wrong folder structure (make sure `api/` and `public/` are folders, not files)
2. Didn't authorize Vercel for GitHub access
3. Typos in file names

Double-check these first!
