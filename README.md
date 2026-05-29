# AI-Driven Semiconductor Market Intelligence

Static website for US-listed AI data center and semiconductor market intelligence.

## Files

- `index.html` - production dashboard.
- `market_feed.json` - structured research payload used by the dashboard process.
- `vercel.json` - Vercel static deployment headers and routing configuration.
- `cloudbaserc.json` - CloudBase static hosting deployment configuration.

## Local Preview

```bash
python3 -m http.server 4173
```

Then open `http://127.0.0.1:4173/index.html`.

## Deploy To Vercel

This is a no-build static site. Connect the GitHub repository to Vercel and use the project root as the output directory. `index.html` is the entry point and `vercel.json` supplies the static-site headers.

## Deploy To CloudBase

This is a no-build static site for CloudBase Hosting.

```bash
export TCB_ENV_ID=your-cloudbase-env-id
tcb app deploy ai-semiconductor-market-intelligence -e "$TCB_ENV_ID" --framework static --install-command "" --build-command "" --output-dir ./ --deploy-path / -f
```

The CloudBase config uses `framework: static`, no install command, no build command, `outputDir: ./`, and `deployPath: /`. Keep the real CloudBase environment ID out of git by passing it through the `TCB_ENV_ID` environment variable.

## Data Policy

The current dashboard intentionally uses a US-listed universe only. China A-shares are excluded until source coverage and filing comparability meet the same confidence threshold.

Educational information only. Not financial advice.
