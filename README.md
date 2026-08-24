# AI-Driven Semiconductor Market Intelligence

Static website for US-listed AI data center and semiconductor market intelligence.

## Files

- `index.html` - production dashboard.
- `market_feed.json` - structured research payload used by the dashboard process.
- `vercel.json` - Vercel static deployment headers and routing configuration.

## Local Preview

```bash
python3 -m http.server 4173
```

Then open `http://127.0.0.1:4173/index.html`.

## Deploy To Vercel

This is a no-build static site. GitHub `main` is the production source of truth. Connect the repository to Vercel and use the project root as the output directory. `index.html` is the entry point and `vercel.json` supplies the static-site headers. Future production updates should be committed and pushed to GitHub for Vercel to deploy automatically.

## Data Policy

The current dashboard intentionally uses a US-listed universe only. China A-shares are excluded until source coverage and filing comparability meet the same confidence threshold.

Educational information only. Not financial advice.
