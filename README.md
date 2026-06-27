# Fitness 4 U Swim School — website

A simpler, single-page site for Fitness 4 U Swim School (St Columb Major, Cornwall),
rebuilt from the old multi-page site. Plain HTML and CSS — no build tools, no frameworks.

## Files

| File         | What it is                                            |
|--------------|-------------------------------------------------------|
| `index.html` | The whole page (content + a little JavaScript)        |
| `styles.css` | All the styling                                       |
| `images/`    | Drop photos in here                                   |

## Viewing it

Just open `index.html` in any web browser — double-click it, or drag it into a browser window.

To preview it exactly as a server would (recommended), from this folder run:

```
python3 -m http.server 8000
```

then visit <http://localhost:8000>.

## Publishing it

Upload the whole folder (`index.html`, `styles.css`, `images/`) to any web host —
the same place the current `fitness4uswimcornwall.co.uk` site is hosted will be fine.
There's nothing to "build" or compile.

> Note: the live domain currently has an **expired SSL certificate**. Worth asking
> the host to renew it so the padlock works and the site isn't flagged as insecure.

## Things to update with real details

These are marked so they're easy to find:

1. **Hero photo** — there's a placeholder box in the hero. To use a real photo:
   - Save the image as `images/hero.jpg`
   - In `styles.css`, find the comment *"If you add images/hero.jpg"* and un-comment the line under it
   - In `index.html`, delete the `<div class="photo-placeholder">…</div>` block
2. **Logo** — the wave-and-sun mark is drawn in code. If you'd rather use the real
   Fitness 4 U logo, replace the `<svg>…</svg>` inside `<a class="brand">` with an
   `<img src="images/logo.png" alt="Fitness 4 U">`.
3. **Instagram link** — search `index.html` for `TODO` and paste in the real Instagram URL.
4. **Photos generally** — any section can take a photo; happy to wire more in.

## Where the content came from

All wording is reworked (not copy-pasted) from the existing site's pages: Welcome,
Swimming, Aquafit & Triathlon, Terms/FAQs, Testimonials and Contact. The full Terms
& Conditions aren't shown on the page — the footer notes they're sent on booking,
which keeps the page short. They can be added as a separate page if you'd like.
