# Tile Frames

Static site — no build step. The two studio apps are self-contained HTML
(`*.dc.html`) that load a local runtime (`support.js`) and local fonts.

## Files served
- `index.html` — landing page linking to both studios
- `Mosaic Studio.dc.html` — Mosaic Studio app
- `Brick Studio.dc.html` — Brick Studio app
- `support.js` — runtime (required by both apps)
- `fonts/` — Google Sans Flex

## Push to GitHub
```bash
git init
git add .
git commit -m "Initial commit: Tile Frames"
git branch -M main
git remote add origin https://github.com/<you>/tile-frames.git
git push -u origin main
```

## Deploy to Vercel
1. Go to vercel.com → **Add New → Project**
2. Import the GitHub repo
3. Framework Preset: **Other** · Build Command: *(none)* · Output Directory: `./`
4. **Deploy**

It's a plain static site, so Vercel serves it as-is. The landing page is `index.html`.
Or run `vercel` from the CLI in this folder.
