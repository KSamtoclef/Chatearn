# ChatEarn V4 Modular — Installation

Upload the entire contents of this folder to the root of the existing ChatEarn GitHub repository. Preserve the `assets/css` and `assets/js` folders.

Then run `chatearn_v4.sql` once in the correct Supabase project.

## Files
- `index.html` — complete production page.
- `assets/css/chatearn.css` — existing main styles.
- `assets/css/chatearn-v3.css` — existing V3 additions.
- `assets/js/chatearn-app.js` — existing public application logic.
- `assets/js/chatearn-v3.js` — existing V3 visitor journey, offers and admin additions.
- `assets/js/chatearn-v4-admin.js` — V4 lightweight admin loader.
- `assets/js/push-legacy.js` — current push integration, preserved unchanged for compatibility.
- `assets/js/clarity.js` — existing Microsoft Clarity loader.
- `chatearn_v4.sql` — additive database performance migration.

## Important deployment order
1. Back up the current repository or create a branch.
2. Run `chatearn_v4.sql` in Supabase.
3. Upload every file and folder from this package.
4. Test the branch/preview deployment.
5. Merge only after public and admin testing passes.

## Rollback
Restore the previous `index.html`. The V4 SQL functions may remain because they are additive.
