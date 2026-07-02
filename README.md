# gopal-kabra.github.io

Personal portfolio site for **Gopal Kabra**, Data/Business Analyst with three years of experience across luxury retail, strategy consulting and financial services (Louis Vuitton, CESI, Capgemini), currently finishing an MSc in Management Engineering at Politecnico di Milano.

Live at **[gopal-kabra.github.io](https://gopal-kabra.github.io)**.

## Why this exists

Recruiters who look this up online mostly find a GitHub profile and not much else. This site gives them a proper destination: the story, the work history with real numbers, four projects written up in detail, and a one-click CV download, instead of a résumé PDF with no context around it.

## Pages

| Page | Content |
|---|---|
| `index.html` | Hero, headline stats, three featured projects |
| `about.html` | Background, skills by category, quick facts, certifications and awards |
| `experience.html` | Full timeline: Louis Vuitton, CESI, Capgemini, with quantified bullet points |
| `projects.html` | Four case studies (Railway Predictive Maintenance, MSc thesis, customer segmentation, Nestlé financial analysis) with problem / approach / result |
| `contact.html` | Email, LinkedIn, GitHub, CV download |
| `404.html` | Custom not-found page |

## Stack

Vanilla HTML, CSS and JavaScript. No framework, no bundler, no build step, no dependencies to install — every file here is exactly what ships to the browser.

- **Structure:** five hand-written HTML pages sharing one nav/footer pattern
- **Styling:** a single `css/style.css` built on CSS custom properties (a small design-token system for color, type and spacing), with a warm paper-and-clay palette and IBM Plex Sans/Mono for type
- **Behavior:** one `js/main.js` (under 60 lines) handling the mobile nav toggle, a scroll-reveal effect via `IntersectionObserver`, and the footer year — no libraries
- **Hosting:** static files served directly by GitHub Pages from the `main` branch, no CI/CD needed

## Project layout

```
site/
├── index.html, about.html, experience.html, projects.html, contact.html, 404.html
├── css/style.css        # design tokens + all component styles
├── js/main.js            # nav toggle, scroll reveal, footer year
├── assets/
│   ├── img/               # favicon, profile photo
│   └── cv/                # downloadable CV (PDF)
├── robots.txt
├── sitemap.xml
└── .gitignore
```

## Running locally

No install step. From this folder:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Notes

This repo holds only what's meant to be public: the site itself, the CV PDF and the profile photo. Private source material used to draft the content (résumé bullet bank, raw notes) lives outside this repo and is never committed.
