# HVAC Tools - iOS offline PWA

This package contains two standalone engineering tools:

- `humidity.html` - Humidity & Dew Point Calculator
- `psychrometrics.html` - Psychrometric Toolkit
- `index.html` - app launcher
- `manifest.webmanifest` + `sw.js` - install/offline support

## Install on iPhone / iPad

1. Upload the **contents of this folder** to any static HTTPS host. Keep the folder structure unchanged.
2. Open the hosted `index.html` URL in **Safari** on the iPhone/iPad while online.
3. Wait a few seconds for the first page load so the offline cache can be created.
4. Tap **Share** -> **Add to Home Screen** -> **Add**.
5. Launch **HVAC Tools** from the Home Screen.
6. After one successful online launch, close it, enable Airplane Mode and reopen it to verify offline operation.

## Important

- Do not open the files directly from the iOS Files app if you want installable/offline PWA behaviour. Service workers require HTTPS (or localhost).
- All calculations run in the browser. The app does not send calculation inputs to a server.
- When updating files later, change `CACHE_NAME` in `sw.js` (for example `hvac-tools-v2`) so installed devices refresh the cached version cleanly.
