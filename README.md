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

Initial DealNow import (2026-07-10): 120 images pulled from the rendered help center pages that were previously hosted on Scribe / Colony Recorder CDN (cloudimg.io). These are DealNow-owned captures of the DealNow product; Scribe's terms assign content ownership to the customer. HelpScout-native images (cloudfront docs assets) were left in place and migrate later with the full help-center pull.
