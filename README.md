# Do Next website

The two pages Apple requires for the App Store listing:

- `index.html`: the **Support URL**
- `privacy.html`: the **Privacy Policy URL**

Kept separate from the app's code on purpose: GitHub Pages is free only for public repos, and the app's code should stay private.

## Putting it online (once, about 10 minutes)

1. Make a free GitHub account if there isn't one. A neutral name like `donextapp` keeps a real name out of the web address.
2. Make a new **public** repository called `donext`.
3. Upload `index.html`, `privacy.html` and `style.css` (Add file → Upload files → Commit).
4. Settings → Pages → Source: "Deploy from a branch", Branch: `main`, folder `/ (root)` → Save.
5. After a minute or two the pages are at:
   - Support: `https://<account>.github.io/donext/`
   - Privacy: `https://<account>.github.io/donext/privacy.html`
6. Put those two links in App Store Connect (App Information → Privacy Policy URL; the version's Support URL), and tell Claude, so the app can link to them too.

## Before launch, check

- If the Apple Watch app doesn't ship in 1.0, take the Watch question off the support page and the Watch lines off the privacy page.
- Any change to what leaves the phone means changing `privacy.html` (and the app's Privacy page) in the same change.
