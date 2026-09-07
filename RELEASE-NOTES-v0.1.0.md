# Micronegative 0.1.0 — macOS (Apple silicon)

First public build. Unsigned: right-click → **Open** the first time, or run
`xattr -dr com.apple.quarantine /Applications/Micronegative.app`.

## In this build

- **RAW import that doesn't touch your originals.** Browsing reads the preview the camera already
  embedded rather than demosaicing — a 42MB Leica DNG opens in ~50ms, against ~2s before — and the
  original file is kept byte for byte instead of being replaced by a larger PNG.
  Tested on Fujifilm RAF (X-Trans), Sony ARW, Leica and Samsung DNG.
- **Capture time, camera and lens** read at import, so a shoot sorts by when it was taken rather
  than the order files were dragged in.
- **Index a folder in place.** Point the Gallery at a folder and it catalogues the photographs where
  they are — thumbnails and metadata only, nothing copied. Chromium-only (File System Access API).
- **Colour Wander influence overlay** — see exactly where the tool is reaching.
- **Grain loupe** rebuilt as a pie of film stocks, 50 to 3200 ISO, one setting per slice.
- Fixed: sliders could jump to 100% if a background task rebuilt the panel mid-drag.
- Fixed: Bokeh and Anamorphic did nothing until hidden prerequisites were met.
- Fixed: preview windows kept showing the previous photograph until the tool was reopened.
- Faster: Clarity/Texture drags ~19% cheaper; Colour Wander drags 12× cheaper.

## Requirements

macOS 10.12+, Apple silicon. ~490MB download — the AI models ship inside the app so it works offline.
