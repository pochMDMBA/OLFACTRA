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


## Latest UI and authentication updates
- Toast notifications now appear in a consistent bottom-centre position, within mobile safe areas.
- Removed the redundant “Scoring details (optional)” footer disclosure; the live score breakdown remains in the score panel.
- Updated auth form button contrast for theme-aware readability.
- New registrations explicitly redirect to the currently deployed OLFACULATOR page after email confirmation; URL session detection is enabled with the implicit browser flow, which suits this static client-side app and returns a session to the page after email confirmation.
- The app can also process Supabase email `token_hash` callback links and clean the callback parameters after a session is established.

### Supabase redirect URL configuration
In Supabase Dashboard → Authentication → URL Configuration, make sure the deployed OLFACULATOR URL (including its path, if applicable) is in the Redirect URLs allow-list. Set Site URL to the canonical deployed website address. Confirmation links generated before this update will retain their old redirect destination; test with a newly registered email or resend a confirmation after deployment.
