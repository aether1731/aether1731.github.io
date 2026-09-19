# Portfolio — Md. Iftekhar Alam

Personal portfolio site. Computer Science and Engineering, Islamic University of Technology.

**Live site:** https://aether1731.github.io/

Single HTML file, no build step, no dependencies beyond two webfonts.

---

## Running it locally

Open `index.html` in a browser. That's it.

## Publishing to GitHub Pages

The repository must be named `aether1731.github.io` for the site to live at the root domain.

```bash
cd portfolio
git init
echo ".DS_Store" >> .gitignore
git add .
git commit -m "Portfolio site"
git branch -M main
git remote add origin https://github.com/aether1731/aether1731.github.io.git
git push -u origin main
```

Then on GitHub: **Settings → Pages → Source: Deploy from a branch → Branch: `main` / `(root)` → Save.**

Give it a minute, then the site is live at `https://aether1731.github.io/`.

If you'd rather use a differently-named repo, the URL becomes
`https://aether1731.github.io/<repo-name>/` instead — both are fine.

---

## Editing it

Everything lives in `index.html`.

**Add a project** — copy any `<div class="card">` block inside the Projects window and edit the heading, the description, and the `<span class="tag">` chips.

**Add a whole section** — copy a `<section class="window">` block, give it a new `id`, place it in either `col-main` or `col-side`, and add a matching entry to the Start menu list near the bottom of the file. The taskbar button is generated automatically from the window title.

**Change the look** — the colour palette is the `:root` block at the top of the `<style>` section.

The layout is two columns on desktop and a single column on phones. On desktop, JavaScript pins each window to wherever the layout placed it, which is what makes the windows draggable by their title bars without leaving holes in the page.

---

## Structure

```
index.html      the entire site
README.md       this file
```
