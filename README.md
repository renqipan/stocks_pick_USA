# AI-Driven Semiconductor Market Intelligence

Static website for US-listed AI data center and semiconductor market intelligence.

## Files

- `index.html` - production dashboard.
- `market_feed.json` - structured research payload used by the dashboard process.
- `ai_datacenter_analysis.html` - original reference artifact kept unchanged.
- `vercel.json` - static deployment configuration for Vercel.

## Local Preview

```bash
python3 -m http.server 4173
```

Then open `http://127.0.0.1:4173/index.html`.

## Deploy

This is a no-build static site. For Vercel, deploy the repository/root folder directly. The default output is the project root and `index.html` is the entry point.

## Data Policy

The current dashboard intentionally uses a US-listed universe only. China A-shares are excluded until source coverage and filing comparability meet the same confidence threshold.

Educational information only. Not financial advice.
