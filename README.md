# DeepCleanMac

A native macOS utility for reclaiming disk space, uninstalling apps, finding duplicate files and understanding storage usage.

**[Download DeepCleanMac.dmg](https://github.com/deepcleanmac/app/releases/latest/download/DeepCleanMac.dmg)** · [All releases](https://github.com/deepcleanmac/app/releases) · [Website](https://deepcleanmac.github.io/app/)

## Requirements

- macOS 14 Sonoma or later
- Apple Silicon or Intel (universal app)

## Install

1. Download **DeepCleanMac.dmg** from the [latest release](https://github.com/deepcleanmac/app/releases/latest).
2. Open it and drag DeepCleanMac into your Applications folder.
3. Launch it and follow the Full Disk Access prompt.

Already installed? Use **DeepCleanMac › Check for Updates** to update in place.

## Safety and verification

Every release is:

- **Signed** with an Apple Developer ID (Team ID `SLUA7FD7MQ`).
- **Notarized by Apple**, so macOS has checked it for malicious content before it ever reaches you.
- **Scanned on VirusTotal** by dozens of antivirus engines. The full public report for each release is linked below.

| Release | SHA-256 | VirusTotal |
|---|---|---|
| 1.7.3 | `4f8df3dedbb10c7420796c43185ee2b811ad9b6bd8c2b1a1b92425f1aa726f07` | [View scan report](https://www.virustotal.com/gui/file/4f8df3dedbb10c7420796c43185ee2b811ad9b6bd8c2b1a1b92425f1aa726f07/detection) |

### Check it yourself

Confirm the file you downloaded is the exact one published here:

```sh
shasum -a 256 ~/Downloads/DeepCleanMac.dmg
```

The output should match the SHA-256 above. You can also drop the DMG onto [virustotal.com](https://www.virustotal.com) to scan it yourself.

After installing, confirm Apple's signature and notarization:

```sh
spctl -a -vv /Applications/DeepCleanMac.app
```

You should see `source=Notarized Developer ID`.

## Pricing

Downloading and scanning are free. Cleaning, uninstalling and other actions require a license: **$5/year** or **$9 lifetime**, each for one Mac, with a 14-day money-back guarantee. See [pricing](https://deepcleanmac.github.io/app/#pricing).

## Support

Email [deepcleanmac@proton.me](mailto:deepcleanmac@proton.me).
