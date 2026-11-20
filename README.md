# OLFACULATOR · Navigation Icon & Copy Polish

This build continues from AUTH_TOAST_POLISH and retains the Supabase configuration, authentication flow, PWA assets, mobile navigation, Note Relationships layout, and account storage files.

## Updates
- Removed the sentence about using the database as a vocabulary aid from About OLFACULATOR.
- Removed the About footnote containing the phrase “not strict rules”.
- Removed the fragrance-family count beside “Browse Notes By Family”.
- Capitalized the primary score action as “Save This Combination and Score”.
- Added inline SVG vector icons to the top navigation controls.
- On desktop, the navigation controls are icon buttons with explanatory hover/focus tooltips.
- On mobile, the hamburger menu retains visible text labels beside the vector icons.
- The Sign In / Sign Out label uses a very thin dark text outline for readability; the icon and its state remain intact.
- Bumped the service-worker cache version to v7 so installed pages can fetch the updated assets.

## Deploy
Replace the repository root `index.html` and `service-worker.js` with the versions in this project. Preserve the `icons/` folder, `manifest.webmanifest`, and Supabase SQL files. Commit and push to deploy.
