# Prime-Numbers-

Prime-Numbers- is a compact visual experiment built around the question “Do Prime Numbers Have a Pattern?” It presents the topic as an animated browser experience with a play control and includes the local audio file `sky.mp3`.

## Preview locally

Open `index.html` in a browser, or start a local server from the project root:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Project files

- `index.html` — page entry point, visualization markup, and styles.
- `sky.mp3` — accompanying audio asset. Keep it beside `index.html` while the current relative reference is in use, or update the reference if the file moves.

The page links to Dancing Script through Google Fonts; loading that font depends on network access. Check that the page remains readable if the font request is unavailable.

## Editing and review

Inspect the markup and styles in `index.html` to change wording or appearance. The supplied file list does not identify separate stylesheet or theme files. Preserve the audio filename and relative path unless updating the reference is part of the change.

Use the play control to review the experience. Audio autoplay may be restricted by the browser, so do not assume it will start automatically. When changing the visualization, check that its question and explanatory text remain readable and that the play control can be reached and operated with a keyboard.

No deployment provider, build process, or deployment configuration is documented. Review the page and audio asset in the intended publishing context if you publish it; check browser errors and confirm the local asset paths still resolve.