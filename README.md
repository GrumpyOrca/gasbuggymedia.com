# gasbuggymedia.com

The website of **Gasbuggy Media** — an independent web & app studio in New
Mexico. We build our own experiments, and develop yours.

The name honors [Project Gasbuggy](https://en.wikipedia.org/wiki/Project_Gasbuggy),
a 1967 Operation Plowshare nuclear test in the Carson National Forest:
an audacious tool, aimed at an ordinary problem.

## Stack

None. Three hand-built static HTML pages — no framework, no build step, no
dependencies. Fonts load from Google Fonts; everything else is self-contained
or lives in `/assets`.

| File | Purpose |
|---|---|
| `index.html` | Hero (animated buggy loop) + consult form |
| `projects.html` | The test range — current field tests |
| `about.html` | Why "Gasbuggy" |
| `icons.html` | Internal logo option sheet (not linked from the site) |
| `assets/` | Video loops, poster art (see `assets/LICENSE`) |

Light/dark theme follows the visitor's OS preference, with a manual toggle in
the nav (persisted via `localStorage`).

## Development

Open `index.html` in a browser. That's it.

## Deploy

Any static host works — the repo root is the web root.

**GitHub Pages:** Settings → Pages → deploy from `main` / root. The `CNAME`
file points at `gasbuggymedia.com`; add the matching A/CNAME records at your
DNS provider. Delete `CNAME` if deploying somewhere else.

## Consult form

The form posts to [Formspree](https://formspree.io). The endpoint ID in
`index.html` is public by design (any deployed form's endpoint is visible in
page source); abuse is limited by restricting allowed domains in the Formspree
dashboard.

## License

Code is MIT (see `LICENSE`). Artwork, video, and the Gasbuggy Media brand are
all rights reserved (see `assets/LICENSE`).
