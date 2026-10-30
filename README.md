# Prime-Numbers-

A compact visual experiment built around the question “Do Prime Numbers Have a Pattern?” It presents the topic as an animated browser experience with a play control and includes the local audio file `sky.mp3`.

## Preview locally

Open `index.html` in a browser. Alternatively, from the project root, start a local server:

    python -m http.server 8000

Then visit http://localhost:8000. Use the play control to engage with the animated experience and review changes. If the accompanying audio is unavailable, check that `sky.mp3` remains at the referenced relative path.

## Editing the experience

The visualisation is in the root-level `index.html`, and `sky.mp3` is the accompanying audio asset. Keep its reference in sync if replacing the file. No deployment provider or configuration is documented.