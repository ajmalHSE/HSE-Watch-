# HSE WATCH

Mobile-friendly HSE site inspection web application (initial build).

## Publish on GitHub Pages
1. Create a GitHub repository called `hse-watch`.
2. Upload `index.html` into its root (you can also upload this README).
3. Settings → Pages → Build and deployment → Deploy from a branch → `main` → `/(root)` → Save.
4. Visit `https://YOUR-USERNAME.github.io/hse-watch/` when deployed.
5. In the app, click **Connection** and enter your Supabase Project URL and **publishable** key. Do not paste service-role/secret keys or passwords into repository files.
6. Sign in with a user created under Supabase Authentication → Users and configured in `hw_profiles`.

## Requirements
The separate HSE WATCH Supabase SQL setup must already have been run and the correct user permissions and RLS verified. The `hw_*` tables must exist. The HTML loads the Supabase client from `esm.sh`, so it requires Internet connectivity.

## Limitations
This build does not automatically email 6 PM PDFs. The 10:05 AM notification requires the separate scheduled SQL job and is in-app only (not phone push). GitHub Pages is public web hosting; authorization of inspection data must be enforced at Supabase. Obtain company IT approval before live use.
