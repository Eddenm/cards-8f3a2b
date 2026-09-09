# Daily Cards

Training and nutrition cards, set up to install on a phone home screen.

## Files

- `index.html` — home screen with two tiles
- `training.html` — daily training cards
- `nutrition.html` — meal cards
- `manifest.webmanifest` — name, icon and colours used when installed
- `sw.js` — caches the pages so they open with no signal
- `icons/` — home screen icons

## Putting it on GitHub Pages

1. On github.com, create a new repository. Give it an unguessable name such as
   `cards-8f3a2b` rather than something obvious. Public is fine; Pages publishes
   publicly either way.
2. Choose **uploading an existing file**, then drag in everything in this folder,
   including the `icons` folder. Commit.
3. Go to **Settings → Pages**. Under *Build and deployment*, set Source to
   *Deploy from a branch*, branch `main`, folder `/ (root)`. Save.
4. Wait a minute or two, then reload the Pages settings page. The URL appears at
   the top, in the form `https://YOURNAME.github.io/cards-8f3a2b/`.

## Adding it to the home screen

- **iPhone:** open the URL in **Safari** (this does not work in Chrome on iOS).
  Tap Share, scroll down, tap *Add to Home Screen*.
- **Android:** open the URL in Chrome, tap the three-dot menu, tap
  *Add to Home screen* or *Install app*.

Open it once with signal so the pages cache. After that it works offline.

## Changing it later

Edit the file on GitHub, or upload a replacement, and the site updates within a
minute. The phone may keep showing the old version until the cache refreshes —
to force it, open `sw.js`, change `daily-cards-v1` to `daily-cards-v2`, and
commit that too.

## A note on privacy

GitHub Pages sites are public to anyone with the link, and a private repository
does not change that. There is a `noindex` tag on each page so search engines
should skip it, but treat the URL itself as the only thing keeping it quiet.
