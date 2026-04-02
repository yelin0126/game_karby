# game_karby

## Supabase shared data setup

1. Create a free Supabase project.
2. In the Supabase SQL editor, run `supabase-schema.sql`.
   If you already ran an older version before, run it again to add the latest leaderboard columns and the `guestbook_messages` table.
3. Open `supabase-config.js` and fill in:
   `url: 'https://YOUR_PROJECT.supabase.co'`
   `anonKey: 'YOUR_SUPABASE_ANON_KEY'`
   `leaderboardTable: 'leaderboard_scores'`
   `guestbookTable: 'guestbook_messages'`
4. Commit and push the updated files.

When every local environment points to the same Supabase project, leaderboard scores and guestbook messages become shared across different browsers and different machines.

If `supabase-config.js` is left empty, the game falls back to localStorage-only mode.
