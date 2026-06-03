# rawz.media

Bilingual (English / 中文) marketing site for **RAWZ.** — connecting Western brands with Chinese consumers.

Static site, no build step. Pure HTML/CSS/JS in `index.html`.

## Files
- `index.html` — the whole site (EN/CN toggle, all sections)
- `rawz_icon.svg` — favicon / app icon
- `rawz_logo_primary.svg` — primary wordmark

## Run locally
Just open `index.html` in a browser. Or serve it:
```bash
python3 -m http.server 8000
# visit http://localhost:8000
```

## Deploy with GitHub + Vercel
1. Create a new GitHub repo and push this folder:
   ```bash
   git init
   git add .
   git commit -m "RAWZ.media site v1"
   git branch -M main
   git remote add origin https://github.com/<you>/rawz-media.git
   git push -u origin main
   ```
2. Go to **vercel.com → Add New → Project**, import the repo.
3. Framework Preset: **Other**. Build Command: *(leave empty)*. Output Directory: `./`
4. Click **Deploy**. Every push to `main` auto-deploys.

## Language switch
EN/中文 toggle is in the top-right nav. Choice is remembered (localStorage) and the site auto-detects Chinese browsers on first visit. To edit copy, find paired `<span data-en>…</span><span data-zh>…</span>` in `index.html`.

## Brand
- Magenta `#E9019B` · Near-black `#0A0A0C` · White `#FFFFFF`
- Display: Anton · Body: Inter / Noto Sans SC
