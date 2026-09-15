# Logbook — fitness tracker

A single-page app for logging workouts (exercise, sets, reps, weight, comments) for two profiles, backed by a free Supabase database. No build step — it's one HTML file.

## What's already done
- A Supabase project ("fitness-tracker") is live with two tables: `profiles` (seeded with "Eddy" and "Girlfriend") and `workout_entries`.
- `index.html` is already wired up to that database — nothing to configure.

## Rename the second profile
Go to your Supabase project → Table Editor → `profiles`, and edit the row named "Girlfriend" to her actual name.

## Host it (pick one, both are free)

### Option A — Netlify (drag and drop, easiest)
1. Go to https://app.netlify.com/drop
2. Drag the `index.html` file onto the page.
3. You'll get a live URL in seconds (e.g. `random-name-123.netlify.app`). You can rename it or add a custom domain in the site settings.

### Option B — Vercel
1. Go to https://vercel.com/new
2. Choose "Deploy without Git" / drag-and-drop the file (or push this folder to a GitHub repo and import it).
3. Vercel gives you a live URL.

### Option C — GitHub Pages
1. Create a new GitHub repo, add `index.html` to it.
2. In repo Settings → Pages, set the source to the main branch.
3. Your app will be live at `https://<username>.github.io/<repo>/`.

Bookmark the resulting URL on both your phones (or add it to your home screen) — it'll work like a lightweight app.

## Notes
- There's no login — anyone with the link can see and add entries, which is fine for a private two-person tracker but keep the URL private.
- Data lives in Supabase, so it's the same log no matter which device or browser you open it from.
