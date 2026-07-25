# Español Diario 🇲🇽

A free, offline-capable Spanish learning app for your iPhone. Intermediate level, Mexican Spanish focus.

## What's inside

- **Hoy** — daily dashboard: progress ring, streak, and the day's three tasks
- **Tarjetas** — 12 new vocab words per day (360 total) + spaced-repetition review (SM-2 style) with audio pronunciation
- **Gramática** — one grammar rule per day (30 rules: subjunctive, por/para, se accidental...) with examples and exercises
- **Escucha** — a daily Mexican listening source (N+, Luisito Comunica, No Hay Tos, La Cotorrisa...) with a listening task
- **Práctica** — conjugation drills: 20 essential verbs × 6 tenses
- **Progreso** — streak, XP, 2-week activity chart, vocab mastery, 30-day course map

Everything works offline except the video links. Progress is stored on your phone.

## Host it free (GitHub Pages, ~5 minutes)

1. Create a free account at **github.com** (if you don't have one).
2. Click **+** (top right) → **New repository**. Name it `espanol-diario`, keep it **Public**, click **Create repository**.
3. On the new repo page, click **uploading an existing file**, drag in ALL the files from this folder (`index.html`, `data.js`, `sw.js`, `manifest.json`, and the 3 `.png` icons), then click **Commit changes**.
4. Go to **Settings → Pages** (left sidebar). Under "Branch", select **main**, folder **/ (root)**, click **Save**.
5. Wait ~1 minute. Your app is live at:
   `https://YOUR-USERNAME.github.io/espanol-diario/`

## Install on your iPhone

1. Open that URL in **Safari** (must be Safari).
2. Tap the **Share** button (square with arrow).
3. Tap **Add to Home Screen** → **Add**.

It now opens full-screen like a native app, works offline (after the first load), and keeps your streak/progress on the device.

## Notes

- **Offline**: the service worker caches everything on first visit. Airplane mode works; only the YouTube links need internet.
- **Audio**: the 🔊 buttons use your iPhone's built-in Spanish voice (works offline too).
- **After day 30**: the course loops for review while your flashcard deck keeps scheduling long-term reviews.
- **Updating content**: edit `data.js` (it's plain, readable data — add days, words, or swap media links), commit on GitHub, and bump the version string in `sw.js` (`espanol-diario-v1` → `v2`) so phones pick up the change.
- **Progress reset**: bottom of the Progreso tab.
