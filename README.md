# Foster Ware IV — Academic CV

Polished academic / professional site built on the [HugoBlox Academic CV](https://github.com/HugoBlox/hugo-theme-academic-cv) template.

**Live site:** https://efdubya4.github.io/academic-cv/

**Profile README (companion):** https://github.com/efdubya4

## Local development

Requirements:

- [Hugo Extended](https://gohugo.io/installation/) `0.162.x` (see `hugoblox.yaml`)
- Node.js 22+ and [pnpm](https://pnpm.io/) (for Tailwind)

```bash
# Install JS deps (Tailwind CLI)
pnpm install

# Run local server
hugo server

# Production build
hugo --minify
```

Site config lives under `config/_default/`. Author profile / resume data: `data/authors/me.yaml`.

## Updating content

| What | Where |
| --- | --- |
| Bio, experience, skills, awards | `data/authors/me.yaml` |
| Homepage sections | `content/_index.md` |
| Experience page layout | `content/experience.md` |
| Projects | `content/projects/*/index.md` |
| Site name / colors / SEO | `config/_default/params.yaml` |
| Nav links | `config/_default/menus.yaml` |
| Downloadable CV PDF | `static/uploads/resume.pdf` |
| Deploy host | `hugoblox.yaml` (`deploy.host: github-pages`) |

## TODOs for you

Search the repo for `<!-- TODO` — remaining gaps:

- Exact internship details you still want to refine
- Project demo/repo links (where still placeholder)
- Portfolio URL and Twitter/X (optional)

Replace `static/uploads/resume.pdf` anytime to update the Download CV button.

## Deployment

Pushing to `main` triggers `.github/workflows/deploy.yml` (Hugo build → GitHub Pages).

First-time Pages enablement: **Settings → Pages → Source: GitHub Actions**.
