# Samruddhi Satpute — Portfolio

A single-page portfolio built around an "API console" theme — fitting for a
backend developer. No framework, no build step: just HTML, CSS, and vanilla JS.

## What's inside
```
index.html   → all content/markup
style.css    → design tokens + all styling
script.js    → typing animation, scroll effects, contact form
assets/hero.jpg → your photo, used as the hero background only
Samruddhi_Satpute_Resume.pdf → your résumé (linked from the "Download résumé" button)
```

## Run it locally
No setup required — no Node, no npm, no dependencies to install.

**Easiest:** double-click `index.html` to open it in your browser.

**Recommended (avoids some browser quirks with fonts/paths):**
```bash
cd portfolio
python3 -m http.server 8000
# then open http://localhost:8000
```
(Any static server works — `npx serve`, VS Code's "Live Server" extension, etc.)

## Deploy it (all free, all static — pick one)

### Option A — Netlify (fastest)
1. Go to https://app.netlify.com/drop
2. Drag the whole `portfolio` folder onto the page.
3. Done — you get a live URL immediately. Add a custom domain later if you want.

### Option B — GitHub Pages
1. Create a new repo, e.g. `github.com/SamrudhiSatpute/portfolio`.
2. Push these files to the `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Portfolio site"
   git branch -M main
   git remote add origin https://github.com/SamrudhiSatpute/portfolio.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Source → Deploy from branch → main → / (root)**.
4. Your site goes live at `https://samrudhisatpute.github.io/portfolio/`.

### Option C — Vercel
1. Go to https://vercel.com/new, import the folder/repo.
2. Framework preset: **Other** (it's static, no build command needed).
3. Deploy.

## Things you'll likely want to personalize
- Swap the GitHub project links (currently pointing to your profile) for the
  actual repo URLs once those projects are pushed.
- Replace `Samruddhi_Satpute_Resume.pdf` with an updated résumé any time —
  keep the same filename and the download button keeps working.
- The contact form has no backend (it's a static site), so it opens the
  visitor's email client pre-filled with their message. If you want real form
  submissions without writing a backend, drop-in services like Formspree or
  Web3Forms work with a single `<form action="...">` change.

## Browser support
Modern evergreen browsers (Chrome, Firefox, Safari, Edge). Respects
`prefers-reduced-motion` — animations are skipped for visitors who have that
OS setting on.
