# seyoonk.com

Personal website for Seyoon Kim. Built with plain HTML and CSS — no frameworks, no build tools. Intentionally simple to make it easy to learn and modify.

---

## File Structure

```
seyoonk.com/
├── index.html       ← Landing page
├── about.html       ← About page
├── projects.html    ← Projects list
├── style.css        ← All styles (shared across pages)
└── README.md        ← This file
```

---

## How to edit

**To update copy (text):** Open the relevant `.html` file and edit the text directly inside the HTML tags. For example, to change your bio on the About page, open `about.html` and find the `<p>` paragraphs inside `<div class="about-content">`.

**To change styles:** All visual styling lives in `style.css`. The file is organized into sections with comments. Find the section for the element you want to change.

**To add a project:** Open `projects.html`. Find the comment block labeled `TEMPLATE` and copy the `<li class="project-item">` block above it. Fill in your project name, link, year, description, and tags.

---

## How to preview locally

Open any `.html` file directly in a browser — just double-click it. No server needed for a static site like this.

For a more accurate local preview (especially for relative links), run a simple local server:

```bash
# With Python (usually pre-installed on Mac/Linux)
python3 -m http.server 8000

# Then open: http://localhost:8000
```

---

## How to deploy

This site is hosted on Netlify, connected to this GitHub repo. To deploy a change:

```bash
git add .
git commit -m "describe what you changed"
git push
```

Netlify detects the push and automatically rebuilds and deploys the site. Changes are live within ~30 seconds.

---

## Working with Claude Code (CLI)

Once you've installed Claude Code, you can open a terminal in this folder and describe changes in plain English:

```bash
claude "add a new project card for my new app — it's called X, built in 2026, one-line description is Y"
claude "update my bio on the about page"
claude "change the accent color to slate blue"
```

Claude Code will edit the files directly. Review the diff, then push to deploy.

---

## Future ideas

- [ ] Add a favicon
- [ ] Add Open Graph tags (for link previews on Slack/Twitter)
- [ ] Add a dark mode toggle
- [ ] Add individual project pages
- [ ] Add a simple contact form
