# cyan.fish

Static personal site served via Cloudflare Worker using [Workers Static Assets](https://developers.cloudflare.com/workers/static-assets/).

## Develop locally

```bash
npm install
npm run dev
```

## Deploy manually

```bash
npm run deploy
```

Requires a Cloudflare account and `wrangler` auth (`npx wrangler login`).

## Deploy via GitHub Actions

Pushes to `main` deploy automatically.

Set these repository secrets in **Settings → Secrets and variables → Actions**:

- `CLOUDFLARE_ACCOUNT_ID` — found in the Cloudflare dashboard right-hand sidebar
- `CLOUDFLARE_API_TOKEN` — create one at **My Profile → API Tokens → Create Token** using the **Edit Cloudflare Workers** template
