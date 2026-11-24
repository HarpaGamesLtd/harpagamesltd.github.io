# Black Hole Evolution website

A static site: the game's home page and its privacy policy. It gives the stores and AppLovin the "website" and "privacy policy" links they ask for, and it is where `app-ads.txt` will live.

| File | What it is |
|---|---|
| `index.html` | Home page |
| `privacy.html` | Privacy policy (Firebase Analytics, AppLovin MAX, Google AdMob/UMP, ATT, purchases) |
| `style.css`, `icon.png`, `favicon.png`, `screenshot.jpg` | Style and images |
| `app-ads.txt` | Authorized ad sellers (IAB). Google AdMob line since 2026-11-24; add AppLovin and each mediated network's lines when they are connected (ad-monetization-manager) |

**Live:** https://harpagamesltd.github.io/ (policy: https://harpagamesltd.github.io/privacy.html), GitHub Pages from `HarpaGamesLtd/harpagamesltd.github.io`, branch `main`, published as Harpa Games.

## Rules
- Only "Harpa Games, a brand of Italek Ltd" (with Italek's registered company details where the law needs them, e.g. the privacy policy's data controller) and `harpagamesltd@gmail.com` appear on the site and in its repository. No personal names, usernames or personal emails (owner, 2026-11-08; Italek wording approved 2026-11-24).
- Have the privacy policy checked by someone qualified before the store launch. It is written from what the game does today, but it isn't legal advice.
- `app-ads.txt` has to sit at the root of the domain, so the site stays at a domain root. A custom domain (e.g. `harpagames.com`) can later point at the same Pages site (Settings → Pages → Custom domain).

## Publishing changes
Commit the change in the game repo, then run `Tools/publish_website.sh`. It pushes this folder as a single commit authored "Harpa Games", so the public history carries no personal details.

Preview locally: `.claude/launch.json` → "website" (http://localhost:8766/).
