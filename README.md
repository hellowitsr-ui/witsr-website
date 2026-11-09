# witsr-website
Official website for WITSR — Why Is This So Ridiculous? (witsr.net)

A static site for GitHub Pages: plain HTML and CSS, no build step, no cookies, no analytics.

## Pages
- `index.html` — homepage (hero buttons: Join the Closed Beta, Submit Feedback)
- `beta/index.html` — closed-beta how-to-join steps + feedback form link (served at `/beta/`)
- `privacy/index.html` — privacy policy (served at `/privacy`)
- `privacy/fr/index.html` — French privacy policy (served at `/privacy/fr/`)
- `404.html` — page not found

## Files
- `assets/css/style.css` — the only stylesheet (light and dark)
- `assets/img/` — WITSR's own artwork (app icon, Clarissa, Teresa, Bob); `assets/img/screens/` — four gameplay screenshots (Android build, 540×1170)
- `assets/fonts/LilitaOne-Regular.ttf` — Lilita One by Juan Montoreano, under the SIL Open Font License 1.1 (`assets/fonts/OFL.txt`)
- `.nojekyll` — serve files as-is (no Jekyll processing)

All links are relative, so the site works both at `hellowitsr-ui.github.io/witsr-website/` and at `witsr.net/`.

## Preview locally
```
cd witsr-website
python -m http.server 8080
```
Then open http://localhost:8080/, http://localhost:8080/beta/ and http://localhost:8080/privacy/

## Custom domain (later)
Add a `CNAME` file containing `witsr.net` only after the domain's DNS points to GitHub Pages.
