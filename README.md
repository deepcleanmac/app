# Promo download page (temporary)

Standalone, noindex download page for BundleHunt and other promotions while the main domain is flagged in Safari.

## Deploy

1. Create a new public GitHub repo (e.g. `deepcleanmac-download`).
2. Create a Release, tag `v1.7.3`, and attach `DeepCleanMac.dmg` (from deepmacclean-web/public/).
3. Fill the placeholders:
   ```sh
   sed -i '' 's#DOWNLOAD_URL#https://github.com/OWNER/REPO/releases/latest/download/DeepCleanMac.dmg#g' index.html
   ```
   The `releases/latest/download/` URL always serves the newest release, so the link never changes when you ship a new version.
4. Push this folder to the repo root. In Settings > Pages, set Source to "Deploy from a branch", branch `main`, folder `/`.
5. Page goes live at `https://OWNER.github.io/REPO/`.

## Notes

- Leave `robots.txt` out. If you block crawlers, they never see the `noindex` tag.
- When you ship an update, attach the new DMG to a new Release. Sparkle updates still come from the main appcast.
