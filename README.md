# pa-kb-assets

Public image assets for the PrivateAuto and DealNow help centers.

Images live here so they carry one permanent URL that serves the HelpScout help center today, the customer AI chatbot, and any future help-center render from the knowledge base repo. Everything in this repo is customer-facing content already published on the public help centers. No PII, no internal-only material.

## Layout

- `dealnow/<article-number>/img-NN.<ext>` — images for DealNow help center articles, foldered by HelpScout article number, numbered in body order at the time of migration.
- `privateauto/<article-number>/...` — same convention for PrivateAuto (migration pending).
- `dealnow/url-swap-map.csv` — old URL to new URL map for the migration (article, old_url, new_url). The Article Agent applies swaps per batch during the help-center rewrite waves.

## Reference URLs

Embed images via raw URLs:

```
https://raw.githubusercontent.com/PrivateAuto/pa-kb-assets/main/dealnow/<article>/img-NN.png
```

## Provenance

Complete DealNow import (2026-07-10): 219 images. Every image from all 46 published DealNow articles (65 previously HelpScout-native + 120 previously on Scribe / Colony Recorder CDN), numbered in body order, plus 34 images from the 5 surviving unpublished drafts (articles 286, 287, 289, 324, 344). This repo is the single home for help-center images going forward: articles reference these paths, and replacing a stale screenshot means overwriting the file at the same path (no article edit needed). All content is DealNow-owned product captures; Scribe's terms assign content ownership to the customer. PrivateAuto images migrate when its article overhaul starts.
