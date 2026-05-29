# California Workforce Indicators Pilot — Viability Findings

A public web version of the Agile Visual Analytics Lab (AVAL) at UCLA's May 2026 report on California's child welfare workforce indicators pilot. Findings, per-indicator viability ratings, and options for next steps.

**Live page:** https://YOUR-USERNAME.github.io/REPO-NAME/

## What's in this repository

- `index.html` — the full report as a single self-contained page. Tabs for Findings and Indicators; the Indicators tab includes a county filter. Locked / read-only.
- `.nojekyll` — tells GitHub Pages to serve the HTML as-is without running Jekyll.

## How to publish (GitHub Pages)

1. Create a new GitHub repository. Name it something readable — `workforce-indicators-pilot` or similar.
2. Upload `index.html` and `.nojekyll` to the repo root. (Drag-and-drop on the GitHub web interface works fine.)
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment," set Source = **Deploy from a branch**, Branch = **main**, Folder = **/ (root)**, then click Save.
5. Wait 30–60 seconds. GitHub Pages will publish the site at `https://YOUR-USERNAME.github.io/REPO-NAME/`.

The site updates automatically on every push to the main branch.

## Updating the page

When the report changes, regenerate `index.html` from the AVAL infographic-report skill (see your local `~/.claude/skills/infographic-report/`), then commit the new file. GitHub Pages will redeploy within a minute.

## Brand and attribution

The AVAL @ UCLA logo links to https://aval.ucla.edu on every page. The report's source data and methods are described inline. Suggested citation:

> Agile Visual Analytics Lab at UCLA. (2026, May). *California Workforce Indicators Pilot — Viability Findings.* University of California, Los Angeles.

## License

Set the repository visibility to **Public** so anyone can view the report. If you want to allow re-use of the report content, add a `LICENSE` file (Creative Commons Attribution 4.0 is a common choice for public-sector research outputs).
