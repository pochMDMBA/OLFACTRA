# OLFACULATOR Mobile-ready project

## Deploy
Upload the contents of this folder to the root of your GitHub repository, preserving the `icons/` folder. Vercel should deploy from the same root.

## Add to Home Screen
- **iPhone/iPad:** Open the deployed HTTPS website in Safari, tap Share, then choose **Add to Home Screen**. iOS uses `icons/apple-touch-icon.png` for the installed icon.
- **Android:** Open the deployed HTTPS website in Chrome and use **Install app** or **Add to Home screen** from the browser menu. Android uses `manifest.webmanifest` and the 192px/512px icons.

The web app manifest sets `display: standalone`. A service worker provides a small offline shell and uses network-first navigation so updated deployments are picked up promptly.

## Supabase
The current HTML preserves the existing Supabase browser configuration. Keep the public publishable/anon key in the browser config; never put a service-role/secret key in the HTML. Existing tables and user data are not modified by this mobile update.
