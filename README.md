# Instagram Profile Highlights Downloader (ZIP + Metadata)

Download Instagram profile highlights with media and metadata as an organized ZIP archive. Built for authorized Instagram highlight backup, story archive preservation, profile data export, social media migration, and developer workflows needing structured JSON, images, videos, timestamps, and cover data.

This repository contains the **YouPreserver Highlights Exporter** — a Chrome extension that exports your Instagram story highlights as a ZIP for the [YouPreserver](https://roktimsaha.com) WordPress plugin.

## Features

- Exports all visible story highlights from an Instagram profile you are logged into
- Downloads cover images and story media (images + videos)
- Packages everything in a structured ZIP with JSON metadata
- Compatible with YouPreserver WordPress plugin v1.3.0+

## Install (Chrome, unpacked)

1. Clone or download this repository
2. Open `chrome://extensions`
3. Enable **Developer mode**
4. Click **Load unpacked**
5. Select this folder (the directory containing `manifest.json`)

## Use

1. Log in to Instagram in Chrome
2. Open the Instagram profile whose highlights you want to export
3. Click the extension icon → **Start**
4. Wait for the ZIP download to complete
5. In WordPress: **YouPreserver → Highlights → Import Highlights ZIP**

## Export format

| Path | Description |
|------|-------------|
| `highlights.json` | Manifest with highlight metadata and file paths |
| `files/covers/` | Cover images |
| `files/media/` | Story images and videos |

The JSON includes highlight IDs, titles, sort order, story IDs, media types, timestamps, and relative file paths.

## WordPress import

Upload the exported ZIP in the YouPreserver plugin:

**WordPress admin → YouPreserver → Highlights → Import Highlights ZIP**

The plugin validates the manifest, extracts media, and displays highlights on your public gallery page.

## Requirements

- Google Chrome (Manifest V3)
- Active Instagram login session
- [YouPreserver](https://roktimsaha.com) WordPress plugin for import and display

## License

MIT — see [LICENSE](LICENSE).

## Author

Built by [Roktim Saha](https://roktimsaha.com)
