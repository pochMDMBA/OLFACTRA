# OLFACULATOR · Note Relationships Responsive Update

This build continues from the MOBILE_NAV_GOLD release and preserves the existing Supabase configuration and PWA assets.

## Updates
- Centered the OLFACULATOR logo and wordmark within the mobile banner, reserving space for the existing hamburger menu.
- Renamed Note Database to NOTE RELATIONSHIPS.
- On mobile, Note Relationships is repositioned to the bottom of the fragrance workspace. On desktop, it stays in the existing sticky sidebar location.
- Wrapped the note families from Citrus through Other / Modern Materials in a disclosure. It is collapsed by default on mobile and open by default on desktop. A user's manual toggle is preserved during viewport changes.
- Searching notes automatically opens the note-family list so matching notes remain visible.

## Deploy
Replace the root `index.html` in your GitHub repository with this file. Keep the existing `icons/` directory, `manifest.webmanifest`, and `service-worker.js` alongside it. Commit and push to trigger the normal Vercel deployment.

No Supabase schema or credential changes are required.

The service worker cache has been advanced to `olfaculator-shell-v3` so installed browsers retire the previous shell and request the updated page.
