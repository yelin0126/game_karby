# game_karby

## Supabase leaderboard setup

1. Create a free Supabase project.
2. In the Supabase SQL editor, run `supabase-schema.sql`.
   If you already ran an older version before, run it again to add the `coins` and `final_score` columns.
3. Open `supabase-config.js` and fill in:
   `url: 'https://YOUR_PROJECT.supabase.co'`
   `anonKey: 'YOUR_SUPABASE_ANON_KEY'`
4. Commit and push the updated files.

If `supabase-config.js` is left empty, the game falls back to localStorage leaderboard mode.
