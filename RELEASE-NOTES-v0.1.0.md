# Micronegative 0.1.0 — macOS

**A darkroom that runs on your desk.** First public build.

---

### Load the negative

Drop a card of Sony A1 or Fujifilm frames in and they come up as fast as you can arrow through them.
A 42MB Leica DNG hits the screen in about a twentieth of a second — Micronegative reads the preview
your camera already wrote instead of grinding the sensor data first.

**Your originals are never touched.** Not converted, not replaced, not moved. The file that came off
the card is the file still on the disk when you're done.

Fujifilm RAF, Sony ARW, Leica and Samsung DNG, Canon, Nikon and the rest.

### The light table

Point it at a shoot folder and it builds a contact sheet from what's there — thumbnails and metadata
only, nothing duplicated, nothing quietly filling your drive. Your library stays in Finder exactly
where you left it.

Every frame is read for when the shutter fired, which body, which lens, at what stop. Throw the
files in any order; they land in the order you shot them.

### The grade

Twenty-nine tools, chained, reorderable, maskable, and nothing baked until you export.

**Film Emulation** across measured stocks — Portra, Ektar, Gold, Superia, Provia, Ektachrome — with
push and pull and per-channel toe and shoulder. **Grain** modelled as silver crystals rather than
noise, with a loupe laying out seven stocks from ISO 50 to 3200 so you pick it by eye against your
own frame. **Colour Wander**, letting a colour run out of its saturation points the way a wet
emulsion bleeds, with an overlay showing exactly how far it reaches. **Halation** round the
highlights, **Diffusion** for the filter over the lens, **Cinema Looks** cut from your own picture,
and a **Lens** stage with flare, anamorphic streaks, bokeh shaped by aperture blades and corner
falloff.

Underneath: zones and curves, lift/gamma/gain, HSL and split toning, highlight roll-off, gradient
and radial masks, clone & heal, sky recovery, and a facelift pass that finds the face itself.

### It stays on your machine

Object selection, erase & heal, depth, faces and sky all run locally. The models travel inside the
app, so it works with the network unplugged. No account, no telemetry, nothing uploaded.

---

## Installing

**Unsigned build** — macOS will refuse it the first time.

1. Open the DMG, drag **Micronegative** into Applications.
2. **Right-click → Open → Open.** A double-click won't offer the choice. Once only.

Still refused?

```
xattr -dr com.apple.quarantine /Applications/Micronegative.app
```

macOS 10.12+, Apple silicon. 490MB, because the models come with it.

## Or use it in a browser

Same editor, nothing to install: **[micronegative.com](https://micronegative.com)**
