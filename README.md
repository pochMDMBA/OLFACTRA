# OLFACULATOR v24r1 · Rebuilt from v23

## Changes in this repair
- Rebuilt directly from the original v23 project files.
- Placed the desktop Note Relationships window 16px below the 132px masthead.
- Restored vertical scrolling on the Note Relationships window itself so its individual note relationship entries can be navigated.
- Preserved natural document scrolling for tablet and mobile layouts.
- In My Combinations only, restored Fragrance A and Fragrance B as equal side-by-side left/right columns.
- Removed the individual themed borders and backgrounds around fragrance entries while retaining each fragrance's note-colour swatches and the single centre divider.
- Made no changes to My Collection styling or behaviour.
- Preserved the existing application logic, Supabase configuration, theme system, PWA assets, and database files.
- Advanced the service-worker cache to `olfaculator-shell-v24r1`.

## Deployment
Replace the repository root `index.html` and `service-worker.js` with the files in this project. Keep the `icons` folder, `manifest.webmanifest`, and Supabase SQL files. No database migration is required.
