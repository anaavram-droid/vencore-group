# Vencore — Landing Page

A single self-contained HTML file — all photos are embedded directly in
`index.html` as base64 data, so there's nothing that can go missing or break
if the file gets moved, opened locally, or deployed on its own. No separate
`images/` folder to keep track of.

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
Search the file for these placeholders and swap in the real details if they
haven't been updated yet:
- Phone: `+61 478 723 718`
- Email: `contact@vencore.com.au`
- ABN: `26 699 063 520`
- The quote form currently only shows a success message on submit — wire it
  up to Formspree, Netlify Forms, or your own endpoint to actually receive
  enquiries (search for `form.addEventListener('submit'` in `index.html`).
- The "On Site" gallery currently has 9 photos — add more the same way any
  time by asking for them to be dropped in.
