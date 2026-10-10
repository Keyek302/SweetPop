# Sweet Pop

Match-3 puzzle game. No ads, no paywalls, no sign-in. Plain HTML/JS, no build step.

## Option 1: Install as a phone app (PWA, easiest, free)
1. Push this whole folder to a GitHub repo.
2. Settings > Pages > Deploy from branch > `main` / `/docs`.
3. Open the Pages link on your phone.
   - iPhone (Safari): Share > Add to Home Screen
   - Android (Chrome): menu > Install app

It runs full screen and works offline after the first load.

## Files
- `docs/index.html`: the whole game
- `docs/manifest.webmanifest`, `docs/sw.js`: PWA install + offline
- `docs/icons/`: app icons
- `icon-source-1024.png`: big icon for app store listings
- `capacitor.config.json`, `package.json`: native wrapper setup
