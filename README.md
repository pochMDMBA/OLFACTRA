# OLFACULATOR Mobile Navigation + Gold Winner Update

This build continues from MOBILE_READY and includes:

- A complete rounded metallic-gold S-tier winner treatment with an internal moving shine and warm glow. The former rectangular halo is disabled.
- A collapsible Note Database, closed by default, using native accessible disclosure controls.
- A mobile hamburger navigation menu containing My Library, My Combinations, About Us, and Sign In / Sign Out. Desktop navigation remains horizontal.
- Existing Supabase configuration, PWA manifest, service worker, logos, and icons preserved.

## Deploy
Upload the contents of this folder to the root of the GitHub repository, preserving the `icons/` directory, `manifest.webmanifest`, and `service-worker.js`. Commit and deploy.

## Notes
No database migration is required. The service-worker cache was versioned to v2 so installed browsers replace the previous cached shell. Test the mobile navigation and S-tier animation on a real device after deployment.
