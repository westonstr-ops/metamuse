# MetaMuse

Meta AI + Muse in one app. A WKWebView wrapper around the Meta AI + Muse
merger web app, built to sideload with AltStore.

## How it builds

Pushing to `main` runs GitHub Actions on a Mac runner: it builds the app
unsigned, packages `MetaMuse.ipa`, and publishes it as a GitHub Release.

## Sideload with AltStore

1. Download `MetaMuse.ipa` from the latest Release.
2. In AltStore: My Apps → + → pick the .ipa.
3. AltStore signs it with your Apple ID. Free signing expires every 7 days —
   AltStore refreshes it when your laptop is on the same Wi-Fi.

## What's inside

- `MetaMuse/` — SwiftUI app + the bundled `meta-ai-muse.html` web app.
- `.github/workflows/build-ipa.yml` — the build.
