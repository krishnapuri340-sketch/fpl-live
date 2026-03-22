[README.md](https://github.com/user-attachments/files/26163271/README.md)
# FPL Live — Deploy to iPad (Vercel, Free, No Code)

Follow these steps exactly. Takes about 10 minutes.
After this, your app lives at a web address you can open on any device — iPad, iPhone, laptop, anything.

---

## What you need
- A computer (Mac or Windows) — just for the setup, one time only
- An internet connection
- A free GitHub account — sign up at github.com if you don't have one
- A free Vercel account — sign up at vercel.com (use "Continue with GitHub")

---

## Step 1 — Create a GitHub repository

1. Go to **github.com** and log in
2. Click the **+** button (top right) → **New repository**
3. Name it `fpl-live`
4. Make sure it's set to **Public**
5. Click **Create repository**
6. Leave this page open — you'll need it in a moment

---

## Step 2 — Upload your files

On the GitHub page for your new repository:

1. Click **uploading an existing file** (or drag and drop)
2. Upload these files, keeping the exact folder structure:

```
fpl-live/
├── public/
│   └── index.html        ← the main app
├── api/
│   └── fpl.js            ← the serverless proxy
├── vercel.json           ← Vercel config
└── package.json          ← project info
```

To upload with folders:
- Click **Add file** → **Upload files**
- Drag the entire `fpl-live` folder in
- Click **Commit changes**

---

## Step 3 — Deploy to Vercel

1. Go to **vercel.com** and log in with GitHub
2. Click **Add New Project**
3. Find your `fpl-live` repository and click **Import**
4. Leave all settings as default — don't change anything
5. Click **Deploy**
6. Wait about 60 seconds ⏳
7. Vercel gives you a URL like: `https://fpl-live-abc123.vercel.app`

**That's your app URL. Copy it.**

---

## Step 4 — Open on iPad

1. On your iPad, open **Safari**
2. Type in your Vercel URL (e.g. `https://fpl-live-abc123.vercel.app`)
3. Enter your FPL Team ID and tap **Go Live**

### Tip: Add to Home Screen (makes it feel like an app)
1. Tap the **Share** button in Safari (box with arrow)
2. Tap **Add to Home Screen**
3. Tap **Add**

It now lives on your iPad home screen as a full-screen app icon.

---

## Finding your FPL Team ID

1. Open **fantasy.premierleague.com** in Safari
2. Log in and tap the **Points** tab
3. Look at the URL — it shows something like `/entry/1234567/event/`
4. The number (`1234567`) is your Team ID

---

## FAQ

**Is this really free?**
Yes. Vercel's free tier gives you 100GB of bandwidth per month and unlimited deployments. More than enough for personal use.

**Do I need to keep my computer on?**
No. Once deployed, it runs in Vercel's cloud. Your laptop can be off, you can be anywhere in the world.

**What if something breaks?**
Re-upload the files to GitHub. Vercel automatically redeploys whenever you update files.

**Can I share it with friends?**
Yes — just send them your Vercel URL. They enter their own Team ID and see their own data.

---

## Your files checklist

- [ ] `public/index.html` — the main app
- [ ] `api/fpl.js` — the proxy function
- [ ] `vercel.json` — Vercel routing config
- [ ] `package.json` — project metadata
