# Micronegative 0.1.0 — macOS

The first public build. A darkroom that runs on your own machine.

---

### Your RAWs open instantly

Point it at a card of Sony A1 or Fujifilm frames and they come up as fast as you can arrow through
them. A 42MB Leica DNG is on screen in about a twentieth of a second, because Micronegative reads
the preview your camera already wrote rather than grinding through the sensor data first.

**Your originals are never touched.** Not converted, not replaced, not moved. The file that came off
the card is the file that stays on the disk.

Fujifilm RAF, Sony ARW, Leica and Samsung DNG, Canon, Nikon and the rest.

### Your shoot, in the order you shot it

Every frame is read for when it was taken, which camera, which lens and at what settings. Drop a
folder in whatever order you like — it lands on the light table in the order the shutter fired.

### Point it at a folder and leave the photographs there

Give it a shoot folder and it builds a contact sheet from what it finds: thumbnails and metadata
only, nothing duplicated, nothing filling up your drive. Your library stays where you put it, in
Finder, exactly as you left it. *(In the browser version this needs Chrome, Edge or Opera.)*

### The look

Twenty-nine tools in a chain you can reorder, and switch off a piece at a time.

**Film Emulation** across measured stocks — Portra, Ektar, Gold, Superia, Provia, Ektachrome.
**Grain** built from a real crystal model, with a loupe laying out seven stocks from ISO 50 to 3200
so you pick by eye rather than by number. **Colour Wander**, which lets a colour bleed out of its
own saturation points and along the exposure, with an overlay showing exactly how far it reaches.
**Halation**, **Diffusion**, **Cinema Looks**, and a **Lens** stage with flare, anamorphic streaks,
bokeh and falloff.

Underneath: zones, curves, lift/gamma/gain, HSL, masks, clone & heal, sky recovery and a facelift
pass. All non-destructive, all reversible, none of it baked in until you export.

### On your machine, and it stays there

Object selection, erase & heal, depth, faces and sky all run locally. The models travel inside the
app, so it works with the network off. No account, no telemetry, nothing uploaded.

---

## Installing

The build is **unsigned**, so macOS will refuse it the first time.

1. Open the DMG and drag **Micronegative** to Applications.
2. **Right-click the app → Open → Open.** A double-click won't offer the choice. Once only.

If it still refuses:

```
xattr -dr com.apple.quarantine /Applications/Micronegative.app
```

**Requires** macOS 10.12 or later, Apple silicon. The download is 490MB because the AI models come
with it instead of being fetched later.

## Or use it in a browser

The same editor runs at **[micronegative.com](https://micronegative.com)** with nothing to install.
