# MasoomDev Browser Extensions

Official distribution repository for browser extensions developed by MasoomDev.


## Available extension packages (source downloads)

The following three ZIP files are currently in the repository. These are **repository file downloads**, not published GitHub Release assets. They were reported as working by the developer; manifest/security validation and independent browser testing have not yet been completed.

| Extension | Version | Download ZIP |
|---|---|---|
| Masoom Text Expander | 1.0.4 | [Download](https://raw.githubusercontent.com/shayanmila/MasoomDev-Extensions/main/extensions/Masoom-Text-Expander-v1.0.4.zip) |
| SHEIN Image Downloader | Not confirmed | [Download](https://raw.githubusercontent.com/shayanmila/MasoomDev-Extensions/main/extensions/SHEIN_Image_Downloader.zip) |
| eBay Fee & Profit Calculator | 1.0.3 | [Download](https://raw.githubusercontent.com/shayanmila/MasoomDev-Extensions/main/extensions/eBay-Fee-Profit-Calculator-v1.0.3.zip) |

When formal versioned releases are published, the website download links should be migrated to verified GitHub Release assets.

## Downloading
Visit **[GitHub Releases](https://github.com/shayanmila/MasoomDev-Extensions/releases)** for published, versioned extension ZIP packages. For stable versioned releases, use assets attached to a published release. Until those releases are available, the explicitly listed repository ZIP files above provide direct downloads.

## Installing a ZIP extension on Chrome or other compatible Chromium browsers
1. Download the ZIP file and extract it into a permanent folder.
2. In Chrome, open `chrome://extensions/`.
3. Enable **Developer mode**, then select **Load unpacked**.
4. Select the extracted folder that contains `manifest.json`.

Installing unpacked extensions requires Developer mode. This repository is not a Chrome Web Store listing. Review requested browser permissions before installing.

## Release convention
- Create **one release per extension version** with tag `extension-slug-vX.Y.Z`.
- Attach a tested `extension-slug-vX.Y.Z.zip` containing the working extension files.
- Include features, compatibility, permissions, changelog, installation instructions, and a SHA-256 checksum in release notes.
- Existing releases stay available so users can access older versions.
- Do not publish test builds, credentials, private API keys, or archives that contain user data.
- Do not advertise a direct-download link on the website until its asset is confirmed to exist.

## Repository layout
```
extensions/
  example-extension/
    README.md
    ... extension source files ...
.github/workflows/
  validate-extensions.yml
```

Each extension gets its own folder. Distribution ZIPs belong in **Releases** rather than in Git history, to avoid bloating the repository.

Website: https://masoomdev-website.vercel.app/
