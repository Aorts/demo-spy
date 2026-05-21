# Spaya Demos

Static HTML demos deployed to GitHub Pages.

- `index.html` — landing page that links to both demos
- `Spaya-CRM-Dashboard.html` — CRM dashboard (Priority 2 requirements)
- `landing-page-demo.html` — SaaS landing page demo

## One-time setup

1. Push this repo to GitHub.
2. In the repo: **Settings → Pages → Build and deployment → Source** → set to **GitHub Actions**.
3. Push to `main` (or click "Run workflow" in the Actions tab).
4. The workflow publishes to `https://<username>.github.io/<repo>/`.

## How it works

`.github/workflows/deploy.yml` runs on every push to `main`:

1. Checks out the repo.
2. Uploads the repo root as a Pages artifact.
3. Deploys the artifact to GitHub Pages.

No build step — the files are served as-is.

## Local preview

Just open `index.html` in a browser, or run a tiny static server:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```
# demo-spy
