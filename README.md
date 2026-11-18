# Booth: free photo editor and passport photo maker

One file (`index.html`), no account, no server. Photos are edited inside your browser and never uploaded anywhere.

## Put it online with GitHub Pages (5 minutes)
1. On github.com click **New repository**, name it `booth`, choose **Public**, then **Create repository**.
2. Click **uploading an existing file**, drag in `index.html` (and this README), then **Commit changes**.
3. Go to **Settings → Pages**. Under *Build and deployment* choose **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. After about a minute your editor is live at `https://<your-username>.github.io/booth/`. Share that link with friends and family.

You can also just double-click `index.html` to use it on your own computer.

## What it does
- **Open** by button, drag and drop, or paste (Ctrl+V).
- **Crop** freely or to Square, 4:5, 3:2, 4:3, 16:9, 9:16 or the original shape.
- **Rotate** left/right and **flip** horizontally/vertically.
- **Adjust** brightness, contrast, saturation, warmth and vignette.
- **17 filters** including Greyscale, Black & white, Monochrome, Sepia, Noir, Vintage, Duotone, Cyanotype, Retro and Pop art, with a strength slider.
- **Text** in 23 popular fonts, with colour, size, alignment, bold, italic, outline, shadow and label background. Drag to place.
- **Remove background** with AI that runs on your device, then fill with white, grey, blue, black or any colour, or keep it see-through.
- **Resize** by pixels or percentage, with proportions locked.
- **Passport and ID photos** for the US, UK, Schengen/EU, Singapore, Malaysia, India, Australia, Canada, China, Japan or a custom size, with a face guide and print sheets for 4×6 in, 5×7 in or A4 paper.
- **Compress and resize many photos at once:** drop in a whole folder, pick a size (longest side, width or percentage), format and quality, or keep every file under a limit such as 200 KB. See the saving for each photo and download them all as one ZIP. Camera and location data are removed.
- **Save** as PNG, JPG, WebP (and AVIF where the browser supports it), choose quality and size, or keep the file under a limit such as 240 KB for online applications. Copy to clipboard or share on phones.
- Undo/redo (Ctrl+Z / Ctrl+Shift+Z), hold **Compare** to see the original, **Start over** anytime.

## Visitor and save counts
Booth counts visits and saves anonymously with the free [Abacus](https://abacus.jasoncameron.dev) counter: no cookies, no names, no tracking across sites, and nothing is counted for visitors whose browser sends *Do Not Track* or *Global Privacy Control*. To see your totals, add `#stats` to your site address, for example `https://<you>.github.io/booth/#stats`. Change `COUNTER.ns` near the top of the script to a name only you use, or set `COUNTER.on` to `false` to switch counting off.

Click the Booth logo at any time to go back to the start.

## Good to know
- **Background removal needs the internet the first time.** It downloads an AI model (tens of MB) from IMG.LY's servers; your browser caches it after that. The photo itself is processed on your device.
- The background-removal library (`@imgly/background-removal`) is licensed under **AGPL-3.0**. Free personal and non-commercial use is fine. If you ever turn Booth into a commercial product, review that licence or swap the library.
- Very large photos are reduced to 4096 px on the longest side for smooth editing.
- Passport rules differ by country and change. Always check the official requirements before you submit. Print sheets at 100% size, not "fit to page".
- iPhone HEIC photos open fine on iPhone/Safari. On other browsers, export them as JPG first.

## More studios
Switch between them with the tabs at the top of every page.

**Photo (`index.html`)** also has: Auto enhance; exposure, highlights, shadows, vibrance and tint; sharpen, soften and film grain; borders in any colour and rounded corners.

**Video (`video.html`):**
- Timeline with trim (drag clip ends), split (S), duplicate, reorder by dragging, undo and redo.
- Speed from 0.25× to 4×; photo slideshows with an optional slow zoom; freeze frame; snapshot of any frame.
- Transitions between clips: crossfade, fade through black or white, slide, slide up, wipe, zoom and circle, with adjustable length, on one clip or every clip.
- Per-clip colour looks (B&W, sepia, vintage, warm, cool, vivid, noir) plus brightness, contrast and saturation; zoom, reposition, rotate and mirror to reframe (for example landscape to vertical).
- Sound: per-clip volume with fade in and out; detach a clip's sound to the audio lane; several audio tracks (music, sound effects, detached sound); record a voiceover from the microphone; sound tools: remove vocals (karaoke), isolate voice, clearer speech, remove low rumble, reduce hiss, boost bass.
- Titles with five fonts and fade, pop, slide-up and typewriter animations.
- Export as video (MP4 where supported, otherwise WebM), animated GIF, audio only (M4A or WebM), or a PNG frame.

**360° (`360.html`):** opens stitched 360 photos and videos and stitches raw dual-lens files (for example Samsung Gear 360). Level the horizon, set the starting direction, adjust brightness, contrast, saturation and warmth, add a vignette to views, and hide the tripod with a colour patch or your logo. Views: 360, little planet, tunnel and flat. Save 360 photos with Facebook/Google metadata, pictures of the current view, spin-around and spinning-planet videos from photos, 360 videos and flat videos of one view.

**3D (`3d.html`):** cubes, spheres, cylinders, cones, rings, panels and 3D text; open GLB, glTF, OBJ, STL and PLY; move, rotate and resize with handles, exact numbers or exact sizes in millimetres; snap; mirror; make copies in a row or a circle; Shift-click several objects and group them; colours, finishes, pictures on surfaces and faceted shading; realistic reflections; undo and redo; export GLB, STL (3D printing), OBJ, USDZ (AR on iPhone and iPad), a PNG picture or a turntable video.

### Honest limits
- Exports that involve video or animation record in real time: a 2-minute video takes about 2 minutes.
- "Remove vocals" cancels sound panned to the centre of a stereo mix. It works on many songs but isn't the AI stem separation paid tools use, which needs downloads of several hundred megabytes and powerful hardware.
- iPhone HEVC videos may not play in Chrome on Windows; export them as H.264 MP4 first.
- 3D text supports English letters, numbers and common symbols.

3D and 360 use three.js r169 (MIT), included in `vendor/three/`.

## Updating your GitHub repo
Upload everything in this folder, keeping the folder structure: `index.html`, `video.html`, `360.html`, `3d.html`, `README.md`, the `assets` folder and the `vendor` folder. The new studios must be opened from your GitHub Pages address (or a local server), not by double-clicking, because browsers block their modules on `file://` pages.
