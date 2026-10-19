# Spinola support site

The public support and privacy pages for [Spinola](https://github.com/nsgnoah/spinola), a trivia game for couples on iOS and Android. Served by GitHub Pages at **https://nsgnoah.github.io/ola/**. The same privacy policy is also shown inside the app under "Privacy & support" in the home-screen menu.

## Pages

- `index.html` — support page. What the game is, how to get help (email, with pre-filled "Email support" and "Report a wrong answer" templates), common questions (accounts, wrong answers, starting over, deleting online matches, online play on Android), and a link to the privacy policy.
- `privacy.html` — privacy policy. Spinola has no accounts, servers, analytics, or third-party SDKs. The policy spells out what stays on the device, exactly what a Game Center turn-based match contains and who can see it, how match deletion works on each side, and that the Android app makes no network requests at all.

Both pages are plain static HTML with inline CSS, no JavaScript, no build step, and a dark-mode variant via `prefers-color-scheme`.

## Editing

Edit the HTML and push to `main`; Pages deploys from the root of that branch. When the privacy policy changes, update the "Last updated" line in `privacy.html` and the copy of the policy inside the app.

## Related

Source for the iOS and Android apps is in the [spinola](https://github.com/nsgnoah/spinola) repo.
