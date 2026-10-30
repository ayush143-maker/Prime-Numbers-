# Prime-Numbers-

A compact visual experiment built around the question “Do Prime Numbers Have a Pattern?” It presents the topic as an animated browser experience with a play control and includes the local audio file `sky.mp3`.

## Preview locally

Open `index.html` in a browser, or start a local server from the project root:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>. Use the play control to engage with the experience and review changes. If the audio is unavailable, check that `sky.mp3` remains at the referenced relative path.

## Editing the experience

The visualisation is in the root-level `index.html`, and `sky.mp3` is the accompanying audio asset. Keep its reference in sync if replacing the file. No deployment provider or configuration is documented.

To personalize the visible wording or appearance, inspect and edit the existing markup and styles in `index.html`; the supplied file list does not identify separate stylesheet or theme files. The page links to Dancing Script through Google Fonts, so changing that link affects an external font resource. Keep `sky.mp3` beside `index.html` if retaining its current relative reference, or update the reference when moving or renaming it. Review the play control and audio after making changes.