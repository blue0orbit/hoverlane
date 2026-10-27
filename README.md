# Hoverbandit site

The public web pages for the game Hoverbandit by BlueOrbit, served by GitHub Pages at
https://blue0orbit.github.io/hoverlane/ (the game was called Hoverlane until 2026-10-27; the repository and the URL
keep the old name until the site moves to its own domain).

- `index.html`: the game's home page (head tags, OpenGraph / Twitter cards and the VideoGame JSON-LD follow
  `docs/store/metadata/web.md` in the game repo)
- `press.html`: the press kit (fact sheet, features, key art and icon; screenshots and trailer at launch)
- `privacy.html`: the privacy policy, generated from the game's `docs/store/privacy-policy.md` with
  `node tools/store/privacy-html.mjs` (copy `public/privacy.html` here after each change)
- `404.html`: the not-found page (root-relative links to `/hoverlane/`)
- `sitemap.xml`: the three pages with their real change dates (update `lastmod` when a page changes)
- `robots.txt`: allows everything and names the sitemap; crawlers only read it at a host root, so it counts once a
  custom domain points here

Images: written here by the game repo's `node tools/store/make-icons.mjs` (from the owner's key art in its
`docs/brand/owner-art/`; re-run it after the art changes, then commit them here):
- `og-image.png`: the OpenGraph share image, 1200 x 630 PNG cut from the wide key art (b); `twitter-card.png`: the
  X card, 1200 x 600
- `img/hero-640.webp`, `img/hero-1280.webp`, `img/hero-2000.webp`: the landing page's picture (wide key art a, srcset)
- `icons/favicon-48.png`, `icons/icon-192.png`, `icons/icon-512.png`, `icons/apple-touch-icon.png` (180 x 180): the
  favicon set (`icon-512.png` is also the JSON-LD logo); the square key art, resized
- `press/hoverbandit-banner.webp` (2000 x 791), `press/hoverbandit-wide.webp` (2000 x 1129) and
  `press/hoverbandit-square.webp` (1254 x 1254): the key art as supplied, shown and offered for download in the press
  kit; `press/hoverbandit-icon-1024.png`: the icon download

The game itself is not in this repository.
