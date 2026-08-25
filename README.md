# vote

Static single-page voter tracking app (`index.html`). All tracking data (edits,
vote status, disqualifications) is stored client-side in the browser's
`localStorage` — nothing is sent to a server.

## Deploy to Cloudflare Pages

### Option A — Direct upload (no Git host needed)

```bash
npx wrangler pages deploy . --project-name=vote
```

Re-run the same command after any change to push a new deployment.

### Option B — Git integration (continuous deploy)

1. Push this repo to GitHub/GitLab.
2. Cloudflare dashboard → Workers & Pages → Create → Connect to Git → select
   the repo.
3. Build settings: no build command, output directory `/`.
4. Every push to the connected branch auto-deploys.

## Local preview

```bash
npx wrangler pages dev .
```
