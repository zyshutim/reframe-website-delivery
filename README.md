# Reframe Website Delivery

Delivery date: 2026-10-08 (Asia/Shanghai).
This package matches the accepted version deployed at https://reframe-website.vercel.app/.

## Contents

- index.html: official website.
- updates.html: next-version announcement.
- docs/: official handbook, preview pages, and Beta handbook.
- beta.html: Beta entry.
- assets/, css/, js/: all referenced images, videos, fonts, demo assets, and site code.

## Deploy

This is a static website. No dependency installation or build step is required.
Serve this directory as the site root using Vercel, Nginx, or another static host.
For Vercel: use Other as framework, leave Build Command empty, and serve the root directory.
Preserve relative paths and filenames. Do not enable a catch-all SPA rewrite to index.html.
Use HTTP(S) for preview; opening via file:// can restrict embedded demo requests.

## Verify

Check /, /updates.html, /docs/overview.html, /docs/next-project.html,
/docs/next-graph.html, /docs/next-storyboard.html, /docs/next-manual-sync.html,
and /docs/beta/overview.html. Confirm videos play and screenshots load.
Verify packaged website files with: shasum -a 256 -c SHA256SUMS.txt

## Excluded

Git history, local Vercel account/project bindings, environment files, editor metadata,
design-source, lab experiments, and unused original media are not included.
No deployment credentials are required or included.
