# Joyce Chan — Portfolio Website

A single-page portfolio built for college applications. Everything lives in one
file (`index.html`) — no build step, no dependencies to install. Just upload it
to GitHub and turn on GitHub Pages.

---

## Put it online with GitHub Pages (about 5 minutes)

1. **Make a GitHub account** at <https://github.com> if you don't have one.
2. Click **New repository** (the green button). Name it something like
   `portfolio`. Leave it **Public**. Click **Create repository**.
3. On the new repo page, click **uploading an existing file**.
4. Drag in **every file from this folder** — `index.html`, `.nojekyll`, this
   `README.md`, and the `assets` folder. Click **Commit changes**.
5. Go to **Settings → Pages** (left sidebar).
6. Under **Build and deployment → Source**, choose **Deploy from a branch**.
   Set **Branch** to `main` and the folder to `/ (root)`. Click **Save**.
7. Wait about a minute, then refresh. GitHub shows a link like
   `https://YOUR-USERNAME.github.io/portfolio/` — that's your live site.

> Tip: if you name the repository exactly `YOUR-USERNAME.github.io`, the site
> lives at `https://YOUR-USERNAME.github.io/` with no extra path.

---

## What's in this folder

```
portfolio/
├── index.html        ← the whole website (open this to preview locally too)
├── README.md         ← this file
├── .nojekyll         ← tells GitHub Pages to serve files as-is
└── assets/
    ├── art/          ← drop real artwork images here later
    ├── dance/        ← drop dance photos / video thumbnails here later
    └── docs/         ← drop résumé + PDFs here if you stop using Vercel
```

You can preview the site any time by double-clicking `index.html` — it opens in
your browser.

---

## Updating the content

**Text, facts, links** — open `index.html` in any editor (even GitHub's own
editor in the browser) and search for the words you want to change.

**Artwork & dance tiles** — these are currently styled placeholders (the pink
gradient boxes). To show real images, add the files to `assets/art/` or
`assets/dance/`, then replace a placeholder tile. For example, find:

```html
<div class="plate p1"><span class="cap">01<b>Torn Portrait</b></span></div>
```

and swap in an image background, e.g.:

```html
<div class="plate" style="background-image:url('assets/art/torn-portrait.jpg');background-size:cover">
  <span class="cap">01<b>Torn Portrait</b></span>
</div>
```

**Résumé & PDF links** — the résumé, research, and certificate links currently
point to your existing Vercel site (`joicechan.vercel.app`). They'll keep
working as long as that site is up. If you take Vercel down, put those files in
`assets/docs/` and update the links in `index.html` to point there, e.g.
`href="assets/docs/joyce-chan-resume.docx"`.

---

## A couple of things to double-check

- **Intended major** is listed as *Data Science* — update it in `index.html`
  (search for `Data Science`) if that's changed.
- **Phone number** is intentionally left off the public site for privacy; email
  and Instagram are the contact methods.

---

Fonts load from Google Fonts and the layout is fully responsive, keyboard
accessible, and respects reduced-motion settings. No tracking, no ads, nothing
to maintain.
