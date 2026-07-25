# Vencore — Landing Page

A single-page static site. No build step, no dependencies — just HTML, CSS and two images.

## Deploy to Vercel

**Option A — Vercel CLI (fastest)**
```bash
npm i -g vercel      # if you don't already have it
cd vencore-deploy
vercel               # first deploy, follow the prompts
vercel --prod        # promote to production
```

**Option B — Drag and drop**
1. Go to https://vercel.com/new
2. Drag this whole folder onto the page
3. Deploy — no configuration needed, Vercel auto-detects it as a static site

**Option C — GitHub**
1. Push this folder to a GitHub repo
2. Import the repo at https://vercel.com/new
3. Framework preset: "Other" (or leave on Auto) — no build command needed

## Project structure
```
index.html          the whole site
images/
  reinforcement-onsite.jpg      hero image
  concrete-construction.jpg     selected work image
vercel.json          cache headers + clean URLs
```

## Before you go live
Search the file for these placeholders and swap in the real details:
- Phone: `(03) 0000 0000`
- Email: `estimating@vencore.com.au`
- ABN: `00 000 000 000`
- Address: `Unit 4 / 22 Foundry Rd, Melbourne`
- The quote form currently only shows a success message on submit — wire it up to Formspree, Netlify Forms, or your own endpoint to actually receive enquiries (search for the `form.addEventListener('submit'` block in `index.html`).
- Add more project photos in `images/` and reference them in the "Selected Work" section as needed.
