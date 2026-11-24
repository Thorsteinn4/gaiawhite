# Gaia White Counseling — website

A plain static site: no framework and no build step. Any static host can serve this folder as is.

## Files
- `index.html`: the home page
- `privacy.html`: Notice of Privacy Practices (placeholder; paste Gaia's notice in)
- `styles.css`: all styles
- `images/gaia-white.jpg`: hero photo
- `fonts/`: self-hosted Cormorant Garamond and Figtree (SIL Open Font License)
- `favicon.svg`, `favicon-32.png`, `apple-touch-icon.png`: the "G" monogram
- `og-image.png`: the preview image when the link is shared

## Before launch
1. **Copy.** Search `index.html` for `[` to find every placeholder (session lengths, family fee, insurance, cancellation policy, hours, parking, email).
2. **Photo.** `images/gaia-white.jpg` is 320×400. A larger original, around 1000px wide, would look sharper on big screens. Replace the file and keep the same name.
3. **Contact form.** Replace the `<form>` with Gaia's secure form embed (SimplePractice, Hushmail or similar). Until then, the form tells people it isn't connected and asks them to call.
4. **Map.** It works now without a key. For the official Maps Embed API, create a key restricted to the site's domain and swap the iframe `src` for `https://www.google.com/maps/embed/v1/place?key=YOUR_KEY&q=115+N+College+Ave,Bloomington,IN+47404&zoom=14`.
5. **Privacy notice.** Paste her Notice of Privacy Practices into `privacy.html`.
6. **Domain.** Point the domain at the host, then make `og:image` in `index.html` a full URL (`https://yourdomain.com/og-image.png`).

## Hosting
Staging: GitHub Pages at https://thorsteinn4.github.io/gaiawhite/ (updates on every push to `main`).
Production: a host in Gaia's name. GitHub's terms don't allow Pages as free hosting for a business.
