# OLFACULATOR website setup

OLFACULATOR opens directly into the fragrance workspace. Visitors can browse the note database, build Fragrance A and B, mix and match profiles, and calculate compatibility scores without signing in.

## Current interface

- The masthead is a slim, modern banner with the centered OLFACULATOR wordmark. Workspace and account controls remain inside the banner.
- On desktop, the Note Database rail starts below the masthead and can scroll independently when its content needs more room. The Compatibility Score rail also starts below the masthead, has no internal scrollbar, and keeps the live score, tier, metrics, and **Save this combination and score** button visible together. The bottom-right Theme selector has its own reserved space and will not cover the save button.
- On smaller screens, both side panels return to normal page flow instead of floating over the masthead or the fragrance workspace.
- **About** opens one dismissible dialog containing the rationale for subjective note selection and practical layering guidance. Close it with the X, click outside the dialog, or press Escape.
- **My Library** opens a searchable list of named fragrances. Each fragrance can be dragged onto Fragrance A or B, or loaded with its button.
- **My Combinations** opens a separate area containing named fragrance pairs, their compatibility scores, and tiers. The collection is sorted by score, highest first.
- Each saved fragrance stores its note colours in the profile JSON. Loading a fragrance restores those colours. Saved combinations also include both complete fragrance profiles, including their colour maps.
- Closing buttons use a fixed-size, centered SVG cross so the glyph stays centered regardless of font metrics.

## Guest access and account-only areas

- Guests can browse the note database, build profiles, and calculate live compatibility scores without signing in.
- Saving fragrances or combinations, and opening the private collection panels, requires an account.
- Saving while signed out opens the sign-in/register dialog. After authentication, the pending save resumes.
- There is no guest/local persistence for fragrances or combinations. Guest selections remain only in the open browser session.

## Enable real accounts and cloud saving

1. The delivered `index.html` is already configured with the Supabase Project URL and the public publishable key you supplied. The old `window.OLFACTRA_SUPABASE_CONFIG` name remains supported as a backward-compatible alias. Do not replace the configured values with placeholder text when copying this file to GitHub.
2. In Supabase, open SQL Editor and run `supabase-schema.sql` only if the `fragrances` and `saved_combinations` tables, RLS ownership policies, and authenticated table grants have not already been created. The schema is safe to re-run and does not delete existing rows.
3. In Supabase Authentication > Providers, enable Email. Set the Site URL and allowed redirect URLs to include your deployed website URL.
4. For Google login, enable the Google provider in Supabase and add the Google OAuth Client ID and Client Secret from Google Cloud Console. Set the authorized redirect URI in Google Cloud to the Supabase callback URL shown in the Google provider configuration page. Add your deployed URL to Supabase's allowed redirect URLs.
5. Replace the repository's root `index.html` with the configured `index.html` from this package, commit, push, and let Vercel redeploy.

When Supabase is not configured, guests can still use the calculator. Account-only actions explain that the owner must configure Supabase before sign-in or registration can work.

## GitHub + Vercel

Upload `index.html` to the root of a GitHub repository and import that repository into Vercel as a static site. Use Framework Preset `Other`, no build command, and `./` as the output directory. Vercel will redeploy when you push commits to the connected GitHub repository.

## Security

The browser uses only the Supabase public anon/publishable key. Never add a Supabase service-role key to the HTML file. Keep RLS enabled on both tables. Each row is associated with `auth.uid()` and policies check ownership for select, insert, update, and delete.

## Troubleshooting: permission denied for a saved table

If the website reports `permission denied for table fragrances` or `permission denied for table saved_combinations`, open **Supabase → SQL Editor**, paste and run the contents of `supabase-permissions-fix.sql`.

These grants are for signed-in users only. Keep RLS enabled and keep the ownership policies from `supabase-schema.sql`. Do not grant table access to `anon` and do not disable RLS to work around this error.
