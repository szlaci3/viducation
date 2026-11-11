# Viducation

A growing collection of educational videos. The website is static: serve this repository as the site root, with `index.html` as its entry page. No website build is required.

## Videos

- [How a dental technician makes a bridge](explainers/dental-bridge/dental-bridge.html) — [MP4](explainers/dental-bridge/dental-bridge.mp4), 30 seconds.

Keep each video and its editable sources in `explainers/<video-slug>/`. Add a card to `index.html` for each new video. Use relative links so the site also works under a URL subpath.

## Local preview

Run `python3 -m http.server 8000` from this directory, then open http://localhost:8000.

## Rendering

Run `npm ci`, then `npm run render:dental-bridge`. Rendering requires `/usr/bin/chromium` and ffmpeg; playback of the existing MP4 needs neither. See the video folder's README for source and export details.
