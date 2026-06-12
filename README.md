# My Portfolio — Deployment Guide

## Files included
- `index.html` — About / home page
- `publications.html` — Research papers
- `projects.html` — AI/ML and web projects
- `education.html` — Academic background
- `experience.html` — Internships and work
- `style.css` — Shared stylesheet (do not rename)

## How to customise

### 1. Replace placeholder text
Search for these strings and replace with your real info:
- `Your Full Name` → your name (e.g. Jean-Paul Nguemo)
- `Your Name` → short name for browser tab
- `YN` → your initials (logo + photo placeholder)
- `yourusername` → your GitHub / LinkedIn username
- `your@email.com` → your real email
- `2025 — 2027 (expected)` → update years as needed

### 2. Add your profile photo
Replace the `<div class="photo-placeholder">` with:
```html
<img class="profile-photo" src="data/photo.jpg" alt="Your Name">
```
Create a `data/` folder and put your photo there (square crop, at least 200×200px).

### 3. Add company logos (Experience page)
Create `data/logos/` and add PNG logos (transparent background, ~100×100px).
Replace the text placeholder like `C1` with:
```html
<img src="data/logos/company.png" alt="Company Name">
```

### 4. Fill in your real content
- Publications: replace the sample entries with your actual papers
- Projects: describe your real projects with GitHub links
- Experience: list your actual internships, most recent first

---

## Deploy on GitHub Pages (free)

1. Create a GitHub account if you don't have one
2. Create a new repository named exactly: `yourusername.github.io`
   (replace `yourusername` with your GitHub username)
3. Upload all these files to the repository
4. Go to Settings → Pages → Source: `main` branch → Save
5. Your site will be live at: `https://yourusername.github.io`

That's it — no hosting cost, no server needed. GitHub Pages is free for public repos.

---

## Custom domain (optional, ~$15/year)

If you want `yourname.dev` instead of `yourusername.github.io`:
1. Buy a domain on Namecheap or Google Domains
2. In the repo Settings → Pages → Custom domain, enter your domain
3. Add a CNAME record in your domain's DNS pointing to `yourusername.github.io`

---

## Tips
- Keep the style.css file unchanged unless you want to redesign
- To add a new page, copy any existing .html file and update the nav `class="active"` link
- To add a Resume link, put your PDF in the root folder and link as `href="resume.pdf"`
