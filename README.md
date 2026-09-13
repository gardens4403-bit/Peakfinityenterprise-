# Peakfinity Enterprise — Website

Static one-page site for Peakfinity Enterprise (agricultural import & export:
shea butter, soybeans, cashew nuts).

## Structure

```
index.html          the whole site (HTML + CSS + JS in one file)
images/              product photos and logo files referenced by index.html
```

## Running locally

No build step — just open `index.html` in a browser, or serve the folder
with any static server, e.g.:

```
npx serve .
```

## Deploying

**Vercel (recommended)**
1. Push this repo to GitHub (see below).
2. Go to vercel.com → Add New Project → Import this repo.
3. Framework preset: "Other". Build command: none. Output directory: `.`
4. Deploy. Add your custom domain under Settings → Domains once live.

## Known TODO before real launch

- The contact form (`#quote-form`) currently only shows a local success
  message — it has no backend. Connect it to Formspree, Web3Forms, or a
  Vercel Serverless Function before relying on it for real inquiries.
  See the comment above the form's JS in `index.html` for details.
