# Hosting Astraly legal pages

Static copies live in this folder:

- [privacy.html](./privacy.html)
- [terms.html](./terms.html)

## Publish HTTPS URLs (required for App Store / Play)

Any static host works. Example with GitHub Pages from this repo:

1. Settings → Pages → Deploy from branch → `/legal` or root with these files copied to `docs/` / `gh-pages`.
2. Confirm public URLs look like:
   - `https://<org>.github.io/<repo>/privacy.html`
   - `https://<org>.github.io/<repo>/terms.html`
3. Set app env (no secrets):

```bash
EXPO_PUBLIC_PRIVACY_URL=https://.../privacy.html
EXPO_PUBLIC_TERMS_URL=https://.../terms.html
```

Until those are set, the app links to the relative legal filenames for local preview only.

## LocationIQ attribution

The Privacy Policy includes the required free-tier credit: “Search by LocationIQ.com”.
