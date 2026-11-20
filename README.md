# OLFACULATOR – Reference masthead and S-tier restoration

This release is based on the latest AMBOSS_VIDEO_RESTORE project and preserves the existing account, library, note database, theme selector, PWA icons, manifest and Supabase files.

## Changes in this release

- Restored the reference HTML masthead scale: 64px emblem and 36px OLFACULATOR wordmark on desktop, with responsive tablet/mobile sizing. The wordmark is centered horizontally and vertically within the single-piece graphite banner.
- Preserved the working hamburger menu on mobile.
- Replaced the S-tier visual treatment with the attached reference HTML animation: warm gold metallic rim, pulsing glow, glints and moving specular sweep. The old rectangular halo remains disabled.
- Matched the desktop side-window proportions to the reference: 285px left Note Relationships panel and 290px right score rail, starting below the taller masthead.
- Fixed the Note Relationships summary background so it bleeds to and is clipped by the rounded upper-right and upper-left corners.
- Advanced the service-worker cache to v11.

## Deploy

1. Extract this ZIP.
2. Replace the repository root `index.html` and `service-worker.js` with the included files.
3. Keep the `icons/` folder, `manifest.webmanifest` and Supabase SQL files in the repository.
4. Commit and push to GitHub, then allow Vercel to redeploy.
5. On an installed mobile shortcut, close and reopen OLFACULATOR or remove/re-add it if the browser continues to use an older cached version.

No Supabase schema migration or database reset is required.
