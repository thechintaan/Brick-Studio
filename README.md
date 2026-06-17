# Brick Studio

A static site — no build step. Brick Studio is a self-contained HTML app
(`Brick Studio.dc.html`) that loads a local runtime (`support.js`) and local fonts.
Projects are saved in the browser (localStorage), so each visitor keeps their own mosaics.

## Files served
- `index.html` — entry point; redirects straight into the app (root URL → Brick Studio)
- `Brick Studio.dc.html` — the app
- `support.js` — runtime (required)
- `fonts/` — Google Sans Flex

## Push to GitHub
With GitHub Desktop: review the changed files → write a commit message → **Commit** → **Push**.

Or from the command line:
```bash
git add .
git commit -m "Update Brick Studio"
git push
```

## Deploy to Vercel (one-time setup)
1. vercel.com → **Add New → Project** → import this repo
2. Framework Preset: **Other** · Build Command: *(none)* · Output Directory: `./`
3. **Deploy**

After that, every `git push` redeploys automatically. The root URL opens Brick Studio.
