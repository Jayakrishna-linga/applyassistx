# ApplyAssistX Website

Landing page for ApplyAssistX — Expert-Led Job Applications.

## Project Structure

```
applyassistx/
├── index.html        ← Main website (single-page)
├── vercel.json       ← Vercel deployment config
├── public/
│   ├── logo.png      ← AX icon logo
│   └── logo-text.png ← applyassistx wordmark
└── README.md
```

## Deploy to Vercel via GitHub

### Step 1 — Push to GitHub
```bash
cd applyassistx
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/applyassistx.git
git push -u origin main
```

### Step 2 — Import to Vercel
1. Go to [vercel.com](https://vercel.com) → **Add New Project**
2. Click **Import** on your `applyassistx` GitHub repo
3. Framework Preset: **Other** (no framework needed)
4. Root Directory: `/` (leave as default)
5. Click **Deploy** ✅

### Step 3 — Connect GoDaddy Domain
1. In Vercel project → **Settings → Domains**
2. Add your GoDaddy domain (e.g. `applyassistx.com`)
3. Vercel shows you DNS records — copy them
4. Go to **GoDaddy → My Products → DNS**
5. Add the records Vercel gives you:
   - **Type A** → `@` → Vercel IP (e.g. `76.76.21.21`)
   - **Type CNAME** → `www` → `cname.vercel-dns.com`
6. Save and wait 10–30 min for DNS propagation
7. Vercel auto-provisions SSL 🔒

## Local Preview
Open `index.html` directly in your browser — no build step needed.
