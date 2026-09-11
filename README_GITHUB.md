# HVAC Tools - GitHub Pages deployment

This folder is ready to publish directly with GitHub Pages.

## Recommended setup

1. Create a new **Public** GitHub repository, for example `hvac-tools`.
2. Upload **the contents of this folder** to the repository root. `index.html` must be at the repository root, not inside another folder.
3. Open the repository: **Settings > Pages**.
4. Under **Build and deployment**:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/(root)**
   - Save.
5. Wait for GitHub Pages to publish the site. The URL will normally be:
   `https://YOUR-USERNAME.github.io/hvac-tools/`
6. Open that URL in Safari on iPhone/iPad.
7. Use **Share > Add to Home Screen**.
8. Open HVAC Tools once while online so the service worker can cache all app files. It can then run offline.

## Updating later

Replace the changed HTML/assets in the repository and commit the changes. GitHub Pages will redeploy automatically. If an installed iOS copy seems to show an old version, open the website in Safari once while online, then reopen the Home Screen app.

## Notes

- All calculator logic runs locally in the browser.
- The repository/site is public when using GitHub Free Pages in this setup.
- `.nojekyll` is included so GitHub Pages serves the static files directly without Jekyll processing.
