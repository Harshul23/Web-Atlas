# 🌐 Web-Atlas

![Made with HTML](https://img.shields.io/badge/Made%20With-HTML-orange)
![Made with CSS](https://img.shields.io/badge/Made%20With-CSS-blue)
![Open Source](https://img.shields.io/badge/Open%20Source-Yes-brightgreen)

**Web-Atlas** is a personal, open-source learning hub for web development — a single place to collect class notes, exercises, and small HTML/CSS/JS projects created during courses at Vedam School of Technology.

---

## 📂 What’s in this repository
This repo contains the static site and the resources for your web-development notes:
- `index.html` — homepage / landing page for Web-Atlas
- `notes.html` — notes page (single-page layout for all lectures)
- `style.css` — global styles used by the pages
- `WD_classes/` — folder containing class-specific resources
- (There may be small system files such as `.DS_Store` — safe to remove from the repo.)

> If you want a dynamic notes approach (JSON-driven), add a `data/` folder (for `notes.json`) and a small loader script (`js/notes.js`).

---

## 🚀 Run locally (quick)
1. Clone the repo (SSH):
```bash
git clone git@github.com:Harshul23/Web-Atlas.git
cd Web-Atlas
```

2. Start a simple static server (recommended, so `fetch()` and iframes work correctly):
```bash
# Python 3
python3 -m http.server 8000

# or (Node)
npx http-server
```

3. Open the site in your browser:
```
http://localhost:8000
```

> You can also open `index.html` directly in the browser for simple previews, but some features (CORS, `fetch`) require a static server.

---

## 📦 Deploy with GitHub Pages
1. Ensure `index.html` exists at the repo root (GitHub Pages serves this file).  
2. In GitHub repo → **Settings → Pages** set:  
   - **Branch:** `main` (or `master`)
   - **Folder:** `/ (root)`
3. Save — GitHub will publish at `https://<your-username>.github.io/Web-Atlas/` within a minute or two.

If GitHub Pages shows README instead of the site, double-check that `index.html` is present at the repo root and that Pages is pointed to the root folder (not `/docs`).

---

## 🛠 How to add notes & projects (recommended workflow)
- **Notes (JSON-driven)**: Add a `data/notes.json` file with an array of lecture objects. Use a small client-side loader (`js/notes.js`) to render content dynamically into `notes.html` — this prevents creating dozens of `.html` files.
- **Projects (HTML demos)**: Put each project in `projects/<project-name>/index.html` and reference them from a `data/projects.json`. Use `iframe` preview cards in `projects.html` or “View demo” links to open in a new tab.
- **Static / quick add**: Add files to `WD_classes/` or create markdown/html files inside the repo and link them from `notes.html` manually.

---

## ✅ Contributing
Contributions welcome! A simple flow:
1. Fork this repository
2. Add notes or a project branch (e.g. `feature/add-flexbox-notes`)
3. Push and open a Pull Request describing your changes

Please avoid committing system files like `.DS_Store` — add them to `.gitignore` if necessary.

---

## 📜 License
This project is available under the **MIT License**. See the `LICENSE` file for details.

---

## Contact
**Harshul** — GitHub: [@Harshul23](https://github.com/Harshul23)

