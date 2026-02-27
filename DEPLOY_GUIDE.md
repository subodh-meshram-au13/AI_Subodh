# 🚀 Subodh_AI — Deploy Guide

## What's in this package?
```
subodh-ai/
├── public/
│   └── index.html      ← Your full chat UI
├── server/
│   └── index.js        ← Backend API server
├── package.json
├── Procfile
└── .gitignore
```

---

## STEP 1 — Get Your FREE Anthropic API Key

1. Go to: https://console.anthropic.com
2. Sign up / Log in
3. Click **"API Keys"** → **"Create Key"**
4. Copy the key (starts with `sk-ant-...`)
5. **Keep it secret — never share it!**

---

## STEP 2 — Upload to GitHub (Free)

1. Go to https://github.com and create a free account
2. Click **"New Repository"**
3. Name it: `subodh-ai`
4. Set to **Public**, click **Create**
5. Upload ALL files from this folder (drag & drop in GitHub)

---

## STEP 3 — Deploy on Render.com (Free Hosting)

1. Go to https://render.com and sign up free
2. Click **"New +"** → **"Web Service"**
3. Connect your GitHub account → Select `subodh-ai` repo
4. Fill in settings:
   - **Name:** `subodh-ai`
   - **Build Command:** `npm install`
   - **Start Command:** `node server/index.js`
   - **Plan:** Free
5. Scroll to **"Environment Variables"** → Click **"Add Variable"**
   - Key: `ANTHROPIC_API_KEY`
   - Value: `sk-ant-your-key-here`  ← paste your key
6. Click **"Create Web Service"**
7. Wait 2-3 minutes ⏳

✅ Your URL will be: `https://subodh-ai.onrender.com`

---

## STEP 4 — Custom Domain (Optional)

If you have your own domain (e.g. `subodh.com`):
1. In Render → Your Service → **"Settings"** → **"Custom Domains"**
2. Add your domain
3. Follow the DNS instructions shown

---

## 🎉 Done! Share your URL with friends!

**Your Subodh_AI will:**
- ✅ Chat with real AI (Claude)
- ✅ Remember conversation history
- ✅ Work on mobile
- ✅ Support code formatting
- ✅ Copy & Regenerate messages

---

## Need Help?
- Render Docs: https://render.com/docs
- Anthropic Docs: https://docs.anthropic.com
