# Class Reminder

A single-page web app that shows your next college class, a countdown, room number, and sends browser reminders — no build step, no dependencies to install.

## Deploy on GitHub Pages (free, ~5 minutes)

1. **Create a repo**
   Go to github.com → New repository → name it e.g. `class-reminder` → Public → Create repository.

2. **Upload these files**
   On the repo page, click **Add file → Upload files**, then drag in every file from this folder:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.png`
   - `icon-512.png`
   - `.nojekyll`

   Commit directly to the `main` branch.

3. **Turn on Pages**
   Repo → **Settings → Pages** → under "Build and deployment", set **Source: Deploy from a branch** → **Branch: main**, folder **/ (root)** → **Save**.

4. **Get your URL**
   Wait about a minute, then refresh that same Settings → Pages screen — it'll show a live link like:
   `https://YOUR-USERNAME.github.io/class-reminder/`

## Put it on your phone

1. Open that URL in Chrome (Android) or Safari (iPhone).
2. Tap the browser menu → **Add to Home Screen** (Safari) or **Install app** (Chrome).
3. It now opens full-screen with its own icon, like a real app.
4. On first open, go to **Settings tab → tap a notification toggle** once — your phone will ask for notification permission. Accept it.

## Updating your timetable later

Edit classes right in the app (Timetable tab → tap a class → edit or delete; Settings tab → Add a class). Everything saves on your device automatically — no need to touch GitHub again unless you want to change the app itself.

If you do want to push a code change: edit `index.html` locally, then on the GitHub repo page use **Add file → Upload files** again to overwrite it — Pages redeploys automatically within a minute.

## Known limits (it's a web app, not a native app)

- **Notifications only fire while this tab/app is open** in the background. Browsers can't wake a fully closed tab. Keeping it installed to your home screen and reopening it in the morning is the practical workaround.
- There's no true Android **home-screen widget** (the glanceable "widget" card lives on the Home tab inside the app instead) — that requires a native Android app built with Android Studio or a tool like FlutterFlow/Bolt, which is a different project from this one.
- Your timetable data is stored locally on each device (browser `localStorage`), so it won't sync between your phone and a laptop automatically.
