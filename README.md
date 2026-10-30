# Prime-Numbers-

A compact visual experiment built around the question “Do Prime Numbers Have a Pattern?” It presents the topic as an animated browser experience with a play control and includes the local audio file `sky.mp3`.

## Preview locally

Open `index.html` in a browser, or start a local server from the project root:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Editing the experience

The visualisation is in the root-level `index.html`, and `sky.mp3` is the accompanying audio asset. Keep its reference in sync if replacing the file. No deployment provider or configuration is documented.

To personalize the visible wording or appearance, inspect and edit the existing markup and styles in `index.html`; the supplied file list does not identify separate stylesheet or theme files. The page links to Dancing Script through Google Fonts, so changing that link affects an external font resource. Keep `sky.mp3` beside `index.html` if retaining its current relative reference, or update the reference when moving or renaming it.

## Manual review checklist

These are actions to perform after a change, not verified results:

- Open `index.html` or the local server URL and inspect the experience.
- Try the play control and observe the animated experience. Check that `sky.mp3` loads from the expected relative path and review the audio behavior if you changed the file or its reference.
- Check any image or media paths you changed in `index.html`; keep local references consistent with files beside the page unless you update the paths.
- Inspect the page at narrow mobile-sized and wide desktop-sized viewports. Check that the visualisation and play control remain visible and usable.
- If the Google Fonts link changed, inspect the typography with the external font available and check its fallback appearance if it is unavailable.