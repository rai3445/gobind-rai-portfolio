# Gobind Rai — Portfolio Website

A static, dependency-free portfolio site (HTML/CSS/JS — no build step required).

## Structure
```
index.html         All page content and sections
css/style.css       Design tokens + all styling
js/script.js        Nav, scroll-spy, copy-to-clipboard, contact form, network canvas
assets/             Photo, résumé PDF, and certificate PDFs/images
```

## Run locally
Any static server works, e.g.:
```
python3 -m http.server 8000
```
Then open http://localhost:8000

## Deploy
Drag-and-drop the whole folder onto Netlify, or push it to a GitHub repo and
enable GitHub Pages (root of `main` branch) / Azure Static Web Apps — no build
command needed since everything is plain HTML/CSS/JS.

## Editing content
Everything lives in clearly commented sections inside `index.html`
(HERO, ABOUT, SKILLS, PROJECTS, CERTIFICATIONS, RESUME, JOURNEY, CONTACT).
To add a new project or certificate, copy an existing `<article>` block in
the relevant section and edit the text/links.

## Notes
- GitHub link points to github.com/rai3445 and LinkedIn to the profile linked
  from your résumé — update `js`-free anchor tags in `index.html` (search for
  `github.com` / `linkedin.com`) if either ever changes.
- The contact form has no backend; it opens the visitor's email client via a
  `mailto:` link pre-filled with their message.
