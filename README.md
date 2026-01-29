# Governing AI: Leading Responsible Innovation

**By Shawn Ogunseye**

![Book Cover](cover.png)

> **📚 Living Book**: This is a living document that will be regularly updated as AI governance practices, regulations, and standards evolve.

## Live Site

🌐 **Read online at:** [aigov.ogunseye.com](https://aigov.ogunseye.com)

---

## GitHub Pages Setup

### Step 1: DNS Configuration

Add a **CNAME record** at your DNS provider:

| Type | Name | Value |
|------|------|-------|
| CNAME | `aigov` | `yourusername.github.io` |

Replace `yourusername` with your GitHub username.

### Step 2: GitHub Repository Settings

1. Go to your repo → **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: `main` (or `master`)
4. Folder: `/docs`
5. Custom domain: `aigov.ogunseye.com`
6. ✅ Check **Enforce HTTPS**

### Step 4: Render and Push

```bash
# Render the book (outputs to /docs folder)
quarto render

# Commit and push
git add .
git commit -m "Update book"
git push
```

GitHub Pages will automatically serve from the `/docs` folder.

---

## Quick Start (Local Development)

### Prerequisites

1. **RStudio** (2022.07 or later, includes Quarto)
2. Or install **Quarto** separately: https://quarto.org/docs/get-started/

### Rendering

**In RStudio:**
1. Open this folder as a project
2. Open `_quarto.yml`
3. Click **Render** (or Ctrl+Shift+K)

**Command line:**
```bash
quarto render
```

### Output

Rendered files appear in `_book/`:
- `index.html` - HTML book (start here)
- PDF and EPUB also available

## Project Structure

```
├── _quarto.yml          # Configuration
├── index.qmd            # Front matter & preface
├── cover.png            # Cover image
├── cover-page.tex       # PDF cover page
├── preamble.tex         # PDF styling
├── styles.css           # HTML styling
├── references.bib       # Bibliography
├── chapters/
│   ├── 01-foundations.qmd
│   ├── 02-legal-frameworks.qmd
│   ├── 03-development.qmd
│   ├── 04-deployment.qmd
│   ├── 05-lifecycle.qmd
│   ├── 06-execution.qmd
│   ├── 07-future.qmd
│   └── 08-11 appendices
└── figures/
    └── [16 SVG figures]
```

## Contents

| Part | Chapters |
|------|----------|
| **I. Foundations** | 1. Foundations of AI Governance |
| | 2. Laws, Standards, and Frameworks |
| **II. AI Lifecycle** | 3. Governing AI Development |
| | 4. Governing Deployment and Use |
| **III. Perspectives** | 5. Governance by Design Across the Lifecycle |
| **IV. Advanced** | 6. Governance in Motion |
| | 7. Ongoing Issues and Future Directions |
| **V. Appendices** | A-D. Templates, References, Scenarios, Glossary |

## Version History

| Version | Date | Notes |
|---------|------|-------|
| 1.0 | January 2026 | Initial release |

## License

[![CC BY-NC-ND 4.0](https://licensebuttons.net/l/by-nc-nd/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-nd/4.0/)

This work is licensed under a [Creative Commons Attribution–NonCommercial–NoDerivatives 4.0 International License](https://creativecommons.org/licenses/by-nc-nd/4.0/).

© 2026 Shawn Ogunseye. All rights reserved.

---

*To Dolapo, Tara and Tessa*
