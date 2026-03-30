# Dutch Woorden — Setup Guide

## What's in this folder

| File | What it does |
|------|-------------|
| index.html | The app itself |
| manifest.json | Tells your phone it's an app (name, icon, colors) |
| sw.js | Makes the app work offline |
| icon-192.png | App icon (small) |
| icon-512.png | App icon (large) |

---

## How to put it on your iPhone (5 minutes)

### Step 1 — Create a free GitHub account
Go to https://github.com and sign up. It's free.

### Step 2 — Create a new repository
1. Click the **+** button (top right) → **New repository**
2. Name it: `dutch-woorden`
3. Make sure it's set to **Public**
4. Click **Create repository**

### Step 3 — Upload your files
1. On your new repository page, click **Add file** → **Upload files**
2. Drag ALL files from this folder into the upload area:
   - index.html
   - manifest.json
   - sw.js
   - icon-192.png
   - icon-512.png
3. Scroll down and click **Commit changes**

### Step 4 — Turn on GitHub Pages
1. Click **Settings** (in your repository)
2. Scroll down to **Pages** (in the left sidebar)
3. Under "Source", select **Deploy from a branch**
4. Under "Branch", select **main** and click **Save**
5. Wait 1–2 minutes, then your app is live at:
   `https://YOUR-USERNAME.github.io/dutch-worden`

### Step 5 — Add to iPhone Home Screen
1. Open Safari on your iPhone
2. Go to your GitHub Pages URL above
3. Tap the **Share button** (box with arrow pointing up)
4. Scroll down and tap **"Add to Home Screen"**
5. Tap **Add**

That's it! The app icon now appears on your home screen.
It opens fullscreen, works offline, and remembers your words.

---

## Updating your words

Whenever you add new words to your Excel file:
1. Open the app
2. Go to **Settings**
3. Tap **Replace** next to the file name
4. Upload your new Excel file

Your words update instantly. No need to touch GitHub again.

---

## If you want to update the app itself

If I give you a new version of index.html:
1. Go to your GitHub repository
2. Click on **index.html**
3. Click the **pencil icon** (Edit)
4. Delete everything and paste the new code
5. Click **Commit changes**

The app on your phone updates automatically within a minute.
