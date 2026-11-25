# Promo download page (temporary)

Standalone, noindex download page for BundleHunt and other promotions while the main domain is flagged in Safari.

## Deploy

Live at https://deepcleanmac.github.io/app/ (repo: deepcleanmac/app).

1. Create a Release in this repo and attach `DeepCleanMac.dmg` (from deepmacclean-web/public/).
   The page links to `releases/latest/download/DeepCleanMac.dmg`, so the newest release is always served
   and the link never changes. Keep the asset filename exactly `DeepCleanMac.dmg`.
2. Settings > Pages: Source "Deploy from a branch", branch `main`, folder `/`.

## Notes

- Leave `robots.txt` out. If you block crawlers, they never see the `noindex` tag.
- When you ship an update, attach the new DMG to a new Release. Sparkle updates still come from the main appcast.
