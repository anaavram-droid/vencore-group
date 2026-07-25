# Vencore — Landing Page

A single self-contained HTML file — both photos are embedded directly in
`index.html` as base64 data, so there's nothing that can go missing or break
if the file gets moved, opened locally, or deployed on its own. No separate
`images/` folder to keep track of.

(The trade-off is a larger file — ~880KB instead of ~30KB — since the images
are inline rather than loaded as separate cacheable files. For a landing
page this size that's a fine trade for reliability. If you want the leaner
version with real image files later, just ask and I can split it back out.)

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
2. Drag this folder (containing `index.html` and `vercel.json`) onto the page
3. Deploy — no configuration needed, Vercel auto-detects it as a static site

**Option C — GitHub**
1. Push this folder to a GitHub repo
2. Import the repo at https://vercel.com/new
3. Framework preset: "Other" (or leave on Auto) — no build command needed

## Before you go live
Search the file for these placeholders and swap in the real details:
- Phone: `(03) 0000 0000`
- Email: `estimating@vencore.com.au`
- ABN: `00 000 000 000`
- Address: `Unit 4 / 22 Foundry Rd, Melbourne`
- The quote form currently only shows a success message on submit — wire it up
  to Formspree, Netlify Forms, or your own endpoint to actually receive
  enquiries (search for `form.addEventListener('submit'` in `index.html`).
- Add more project photos as needed (currently just the two supplied).
