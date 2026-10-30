# Prime-Numbers-

Prime-Numbers- is a visual browser experiment asking “Do Prime Numbers Have A Pattern?” The page uses vanilla JavaScript and the Canvas API to render an animation, with a Play button and a local audio file.

## Preview locally

Open `index.html` in a browser, or start a local server from the project root:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## What the visualization shows

The animation computes primes with a sieve and uses the first 2,500 primes in its visualization. It displays the parametric equations `x = p sin p cos p`, `y = p sin² p`, and `z = p cos p`. The animation runs for 48 seconds, followed by a 10-second orbital segment, for 58 seconds total. When it finishes, the Play button becomes Replay.

The page includes the `sky.mp3` audio element and attempts to play it when Play is clicked. The shown controls do not include pause or volume. Keep `sky.mp3` beside `index.html` while the existing relative reference is in use, or update the reference if the file moves.

## Editing and review

Inspect the markup, styles, and scripts in `index.html` to change wording or appearance. The page links to Dancing Script through Google Fonts, so loading that font depends on network access; check readability if the request is unavailable.

Use Play to review the animation and audio behavior, and check that the question and explanatory text remain readable. The page has no documented build process or deployment configuration. If you publish it, include the audio asset at the referenced path and verify the page and asset in the intended context.