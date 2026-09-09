# Vencore Group — Landing Page

A single self-contained HTML file — the logo and all photos are embedded
directly in `index.html` as base64 data. No build step, no dependencies,
no `package.json` needed.

## Push to GitHub

```bash
cd vencore-deploy
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```
(Create the empty repo on GitHub first at https://github.com/new — don't
initialize it with a README there, since you already have one here.)

## Deploy to Vercel from GitHub

1. Go to https://vercel.com/new
2. Import the GitHub repo you just pushed
3. Framework preset: "Other" (or leave on Auto) — no build command needed
4. Deploy

Every future push to `main` will auto-deploy.

## Status
- ✅ Quote form is live — submits to Formspree (`https://formspree.io/f/meaqpnyp`)
  and shows a styled success/error message in place
- ✅ All photos and the logo are embedded, nothing external to break
- ⚠️ First form submission needs confirming — check the inbox tied to the
  Formspree account for a one-time verification prompt after the first test
  submission

## Before you go fully live
Double-check these are the real, final details:
- Phone: `+61 478 723 718`
- Email: `contact@vencore.com.au`
- ABN: `26 699 063 520`
