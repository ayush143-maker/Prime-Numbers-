# Prime-Numbers-

A compact visual experiment built around the question “Do Prime Numbers Have a Pattern?” It presents the topic as an animated browser experience with a play control and includes the local audio file `sky.mp3`.

## Preview locally

Open `index.html` in a browser, or start a local server from the project root:

```sh
python -m http.server 8000
```

Then visit <http://localhost:8000>.

## Editing the experience

The visualization is in the root-level `index.html`, and `sky.mp3` is the accompanying audio asset. Keep its reference in sync if replacing the file. No deployment provider or configuration is documented.

To change visible wording or appearance, inspect the markup and styles in `index.html`; the supplied file list does not identify separate stylesheet or theme files. The page links to Dancing Script through Google Fonts. Keep `sky.mp3` beside `index.html` while its current relative reference is in use, or update the reference if the file moves.

## Configuration and data handling

The listed files include no environment-variable template or configuration file. Do not put passwords, tokens, or other real secrets in `index.html` or assets such as `sky.mp3`. Anything included in browser-delivered resources can be inspected by visitors. No backend or secret-storage mechanism is documented. Review page content and audio assets before committing them to ensure they are suitable for public access and that you have permission to distribute them.

## Troubleshooting

Use these as diagnostic steps; they are not reports of known failures:

1. Confirm `index.html` is the intended entry page and that `sky.mp3` remains beside it if the existing relative reference is unchanged.
2. If the visualization or audio is missing, inspect references in `index.html`, verify the local file is present, and preserve the path relative to the page when moving assets.
3. Open the browser Console and Network panel while loading the page and using the play control. Check for script errors and failed or unexpected requests.
4. Distinguish the local `sky.mp3` file from the Google Fonts request. The font depends on network access; inspect its request separately and check the page's appearance if it is unavailable.
5. If audio does not start automatically, try the play control and review browser messages; do not assume autoplay is permitted.

## Accessibility review checklist

These are future checks, not claims that the page has been tested or found accessible:

- Use a keyboard to reach and operate the play control. Check visible focus and that starting or stopping does not require pointer input.
- Check that the play control has a meaningful accessible name and communicates its action or state.
- Review text, control, and focus-indicator contrast against changing visual backgrounds. Check that the question and explanatory text remain readable.
- If the visualization conveys information, check whether a text explanation communicates its meaning without relying on animation alone.
- Check whether animation can be paused or reduced, including when reduced motion is preferred, and ensure audio remains controllable.