# Micronegative

A local-first, film-look photo editor. RAW and TIFF import, negative inversion, and a full stack of
grading and retouching tools — running entirely on your own machine.

**Nothing is uploaded.** Photographs are read, edited and exported locally; the AI tools run
on-device from models the app downloads once and caches.

**[⬇ Download for macOS](../../releases/latest)** · [Use it in a browser](https://micronegative.com)

---

## What it does

Twenty-nine tools across five stages, applied as a non-destructive chain:

| Stage | Tools |
|---|---|
| **Input** | Exposure Baseline, Colour Calibration, Negative Conversion, Log Conversion |
| **Repair** | Crop & Straighten, Perspective, Lens Corrections, Clone & Heal, Sky Recovery, Facelift |
| **Grade** | Exposure & Colour, Zones, Light Zones, Tone Curve, Lift/Gamma/Gain, HSL & Split Toning, Highlight Roll-off, Masks |
| **Look** | Microfilm, Colour Wander, Film Emulation, Halation, Grain, Cinema Looks, Lenses, Diffusion, Dirt |
| **Output** | Finishing, Export |

Plus a Gallery for importing, rating and picking; and Mono, Print and Restore rooms.

## RAW support

Camera RAW is decoded locally via LibRaw (WebAssembly). Browsing reads the **preview the camera
already embedded** rather than demosaicing the file — a 42MB Leica DNG opens in about 50ms — and
your original file is never modified or discarded.

Tested on Fujifilm RAF (X-Trans), Sony ARW, Leica and Samsung DNG.

## On-device AI

Six models totalling ~330MB, downloaded once on first use and cached — object selection (SAM),
erase & heal (LaMa), depth, face landmarks, subject detection and sky segmentation. You are asked
before anything downloads, and no image data leaves the machine.

## Install (macOS)

The build is **unsigned**, so Gatekeeper will refuse it on first open. To allow it:

1. Download and unzip the release.
2. Move `Micronegative.app` to `/Applications`.
3. Right-click the app → **Open** → **Open** in the dialog. (A plain double-click will not offer
   the option; this is only needed once.)

If macOS still refuses, clear the quarantine attribute:

```
xattr -dr com.apple.quarantine /Applications/Micronegative.app
```

## Browser version

The same application runs at **[micronegative.com](https://micronegative.com)** with no install.
Indexing a folder of photographs in place needs the File System Access API, so that feature is
Chromium-only (Chrome, Edge, Opera); everything else works anywhere.

## Privacy

No accounts, no telemetry, no uploads. Photographs and edits stay in local browser storage or in
the folder you point the app at. The model downloads are the only network requests the editor
makes, and they fetch weights only — never your images.

---

Built by [The Coop](mailto:al@mediacoop.tv). Source is not currently public; this repository exists
to distribute the builds.
