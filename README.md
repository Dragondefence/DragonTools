# Dragon Defence Security Tools

Free security checks from Dragon Defence, built as a single-page web app that can be added to an iPhone or Android Home Screen.

**Email breach check** · **Password check and generator** · **QR code check**

## Hosting

Served with GitHub Pages from the `main` branch (Settings → Pages → Deploy from a branch → `main` / root). Open the site in Safari on iPhone and choose **Share → Add to Home Screen** to install it.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app |
| `manifest.webmanifest` | App name, icons and Home Screen settings |
| `sw.js` | Keeps the app available offline (live checks are never cached) |
| `logo-mark.png`, `logo-wordmark.png`, `logo-full.png` | Dragon Defence logo |
| `apple-touch-icon.png`, `icon-*.png` | App icons |

To show a contact button under each result, set `ctaLink` near the top of the script in `index.html` to the Dragon Defence website or a `mailto:` address.

All checks run in the visitor's browser against public services: XposedOrNot (email breaches), Have I Been Pwned's Pwned Passwords (k-anonymity, so the password never leaves the device), Google and Cloudflare DNS and RDAP (QR link domains). Nothing typed is stored.
