# Organic Store Demo

A static, multi-page website for an organic food store, published with GitHub Pages.

**Live URL:** https://mohammedanasfl.github.io/organic-store-demo/
(available once GitHub Pages is enabled for this repository; see [Publishing](#publishing-with-github-pages))

## Pages

`index.html` (home), `about.html`, `feature.html`, `product.html`, `testimonial.html`,
`blog.html`, `contact.html` and `404.html`.

## Folder structure

```
.
├── LICENSE.txt        License terms for the template files (kept outside docs/, so it is not published)
├── README.md
└── docs/              Everything GitHub Pages serves
    ├── .nojekyll      Tells Pages to serve the files as-is (no Jekyll processing)
    ├── *.html         The eight pages listed above
    ├── css/           style.css (site styles) and bootstrap.min.css
    ├── js/            main.js (site scripts)
    ├── img/           Photos and icons
    └── lib/           Third-party plugins: animate, easing, owlcarousel, waypoints, wow
```

## Run locally

From the repository root:

```bash
python3 -m http.server -d docs 8000
```

Then open http://localhost:8000/.

The pages load jQuery, Bootstrap's JavaScript, Font Awesome, Bootstrap Icons and Google Fonts
from public CDNs, so an internet connection is needed for full styling and interactivity.

## Publishing with GitHub Pages

GitHub Pages cannot be switched on from a commit; it is a repository setting:

1. Open the repository on GitHub, then **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Choose the branch to publish and the **/docs** folder, then **Save**.
4. After the deployment finishes (a minute or two), the site is served at the live URL above.

Because the site lives under `/organic-store-demo/`, all links and asset paths are relative.
Keep them relative when editing, or the site will break on Pages.

## Notes

- The contact form and the newsletter sign-up have no backend; they do not send anything.
- Many navigation and footer links are empty placeholders (`href=""`).
- Text such as "Your Site Name" and the address, phone and email shown on the pages is placeholder
  content to replace.
- `img/favicon.ico` is referenced by every page but does not exist yet, so browsers show no
  tab icon and log a 404 for it.
