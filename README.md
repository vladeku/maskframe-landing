# maskframe.app

The website for [MaskFrame](https://maskframe.app), a privacy utility for iPhone that covers
the personal details in a screenshot before it is shared. Served by GitHub Pages from `main`.

- `index.html` is the home page: icon, tagline, App Store badge.
- `privacy/` and `terms/` are the privacy policy and the terms. The app, its store listing and
  its RevenueCat paywall link to these two addresses.
- `404.html` is the page GitHub Pages serves for any other address.

The app was called SafeShot until 19 September 2026 and its site lived at `getsafeshot.app`,
in `vladeku/safeshot-landing`. That domain was switched off the same day with no redirects,
and the repository is archived; the press kit's source is still there. The two documents do
not mention the old name.

## The OG image

`assets/og.jpg` is rendered by Chrome from `build/og.html`:

```bash
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" --headless=new --hide-scrollbars \
  --force-device-scale-factor=1 --window-size=1200,630 \
  --screenshot=build/og.png "file://$PWD/build/og.html"
```

then converted to JPEG at quality 88 and `build/og.png` deleted. The icon beside it,
`build/icon-1024.png`, comes from `make icon` in the app repository.
