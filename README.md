# Vuja Prompt Vault

A mobile-friendly, installable Progressive Web App containing 256 image prompts from four Vuja Tsoaela packs.

## Publish on GitHub Pages

1. Create a **private or public** GitHub repository. Note: GitHub Pages availability for private repositories depends on your GitHub plan; a published Pages website may be publicly accessible.
2. Upload **all files from this ZIP into the repository root**, not into a nested folder.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, then select **main** and **/(root)**. Save.
5. After GitHub Pages deploys, open the URL shown in Settings → Pages (typically `https://USERNAME.github.io/REPOSITORY/`).
6. On a supported mobile browser, choose **Install app** or **Add to Home screen**.

## Using the app
Select a pack, anime/category, and prompt. Tap **Copy prompt**, then **Open ChatGPT** and paste. Attach a selfie in ChatGPT if desired.

## Important privacy and sales note
**The full paid prompt content is embedded in `index.html`.** Anyone who can access the hosted website can inspect or copy it. Do not publish this complete version publicly if you intend to sell access to the prompts. A private GitHub repository does not automatically make a GitHub Pages site private. For secure paid access, use authenticated delivery instead.

## Updating prompts
The app currently embeds the prompt library in `index.html` so it can work offline. `packs.json` is an editable reference export; modifying it alone will **not** update the app. To change the in-app prompts, update the embedded `PACKS` variable in `index.html` and bump the service worker cache version.

## Included files
- `index.html` — complete app and embedded prompt data
- `manifest.webmanifest` — installable app metadata
- `sw.js` — offline cache
- `icon-192.png`, `icon-512.png`, `icon.svg` — app icons
- `packs.json` — reference data export
- `.nojekyll` — GitHub Pages configuration
- `README.md` — instructions

No backend, API key, or paid hosting is needed for the static app.
