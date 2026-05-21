# Spaya CRM Demo

Static HTML dashboard demo, hosted on GitHub Pages.

- `index.html` — the Spaya CRM dashboard (what the client sees when they open the site)
- `Spaya-CRM-Dashboard.html` — same file, kept under its descriptive name
- `crm-dashboard-requirements.md` — source requirements

## One-time setup

1. Push this repo to GitHub.
2. In the repo: **Settings → Pages → Build and deployment → Source** → set to **GitHub Actions**.
3. Push to `main` (or click "Run workflow" in the Actions tab).
4. The workflow publishes to `https://<username>.github.io/<repo>/` — share that link with the client.

## How it works

`.github/workflows/deploy.yml` runs on every push to `main`:

1. Checks out the repo.
2. Uploads the repo root as a Pages artifact.
3. Deploys the artifact to GitHub Pages.

No build step — files are served as-is.

## Local preview

Just open `index.html` in a browser, or run a tiny static server:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```
# demo-spy
