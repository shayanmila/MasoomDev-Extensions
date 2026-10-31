# Publishing an extension

## Prepare
- Put the complete extension source under `extensions/<extension-slug>/`.
- Ensure `manifest.json` contains the intended name, version, description and only the required permissions.
- Test installation, UI and functionality in a clean browser profile.
- Ensure there are no embedded secrets, copyrighted assets you cannot redistribute, or suspicious downloads.

## Package
Compress the **contents** of the extension folder so that `manifest.json` is at the root of the ZIP. Name it `<extension-slug>-vX.Y.Z.zip`.

## Release on GitHub
1. Open the repository's Releases section.
2. Select **Draft a new release**.
3. Create tag `<extension-slug>-vX.Y.Z` from `main`.
4. Attach the tested ZIP, describe permissions and changes, and publish.
5. Confirm the download works.
6. Add the exact release asset URL to the MasoomDev website directory.

Don't modify or rebuild unrelated extensions when updating one package.
