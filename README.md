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

To change visible wording or appearance, inspect the existing markup and styles in `index.html`; the supplied file list does not identify separate stylesheet or theme files. The page links to Dancing Script through Google Fonts. Keep `sky.mp3` beside `index.html` if retaining its current relative reference, or update the reference if the file moves.

## Browser and platform reliability checklist

This is a checklist for future review, not a record of completed testing or verified compatibility:

- Review the page in current browsers relevant to its intended audience and its HTML/CSS/JavaScript stack. Do not treat a successful review in one browser as evidence for other browsers.
- Open developer tools and inspect the Console and Network panels while loading the page and using the play control. Investigate JavaScript errors, failed requests, and unexpected warnings.
- Check the `sky.mp3` reference against the local file beside `index.html`. Inspect other local and remote references in the page, including the Google Fonts request, and verify paths and requests in the Network panel. Check the appearance when the font is unavailable and consider browser restrictions on audio playback; verify audio through an explicit user action rather than assuming it will autoplay.
- Inspect the page at narrow mobile-sized and wide desktop-sized viewports. Check that the visualization and play control remain visible and usable, and that animation does not obscure content or controls.
- After changing the animation, audio, or resource references, revisit the affected behavior in the relevant browsers. No compatibility or asset-loading results are recorded here.

## Accessibility review checklist

These are future checks, not claims that the page has been tested or found accessible:

- Use a keyboard to reach and operate the play control. Check that focus is visible and that starting or stopping the experience does not require pointer input.
- Check that the play control has a meaningful accessible name and communicates its action or state. Review any separate audio control if one is present in the page.
- Review text, control, and focus-indicator contrast against changing visual backgrounds. Check that the question and explanatory text remain readable.
- If the visualization conveys information, check whether a text explanation or other alternative communicates its meaning without relying on animation alone. Provide appropriate alternatives for informative images added later.
- Check whether animation can be paused or reduced, including when the user's reduced-motion preference is active. Ensure audio remains understandable and controllable during review.