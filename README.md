# Sweet Pop

Match-3 puzzle game. No ads, no paywalls, no sign-in. Plain HTML/JS, no build step.

## Option 1: Install as a phone app (PWA, easiest, free)
1. Push this whole folder to a GitHub repo.
2. Settings > Pages > Deploy from branch > `main` / `/docs`.
3. Open the Pages link on your phone.
   - iPhone (Safari): Share > Add to Home Screen
   - Android (Chrome): menu > Install app

It runs full screen and works offline after the first load.

## Option 2: Real native app with Capacitor (Android Studio / Xcode)
Needs Node.js. Android needs Android Studio, iOS needs a Mac with Xcode.

    npm install @capacitor/core @capacitor/cli @capacitor/android @capacitor/ios
    npx cap add android      # and/or: npx cap add ios
    npx cap sync
    npx cap open android     # or: npx cap open ios

Then build/run from Android Studio or Xcode. After any change to `docs/`, run `npx cap sync`.
Publishing: Google Play has a one-time $25 fee, Apple Developer is $99/year.
Change `appId` in `capacitor.config.json` to your own (e.g. com.yourname.sweetpop) before publishing.

## Files
- `docs/index.html`: the whole game
- `docs/manifest.webmanifest`, `docs/sw.js`: PWA install + offline
- `docs/icons/`: app icons
- `icon-source-1024.png`: big icon for app store listings
- `capacitor.config.json`, `package.json`: native wrapper setup
