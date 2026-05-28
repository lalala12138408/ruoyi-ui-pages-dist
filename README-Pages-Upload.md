# Cloudflare Pages Upload Notes

This directory can be uploaded directly to Cloudflare Pages.

Path:

`C:\Users\Polaris\Documents\Codex\2026-05-23\new-chat-3\ruoyi-ui-pages-dist`

## Included Files

- `index.html`
- `404.html`
- `assets/`
- `_headers`
- `_redirects`

## Why `_headers` matters

It prevents Cloudflare from caching `index.html`, so the SPA shell is always fetched fresh.

Recommended rules:

```txt
/index.html
  Cache-Control: no-store

/404.html
  Cache-Control: no-store

/app/*
  Cache-Control: no-store

/assets/*
  Cache-Control: public, max-age=31536000, immutable
```

## Upload Settings

- Framework preset: `None`
- Build command: empty
- Build output directory: `/`

