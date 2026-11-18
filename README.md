# Booth: free photo editor and passport photo maker

One file (`index.html`), no account, no server. Photos are edited inside your browser and never uploaded anywhere.

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

**Video (`video.html`):** add videos, photos and music; trim by dragging the ends of a clip; split at the playhead; change speed from 0.25× to 4×; turn photos into a slideshow with a slow zoom; add titles in five styles; fade between clips; choose 16:9, 9:16, square or 4:5 at up to 1080p. Export plays your video through once while it records, then saves an MP4 (or WebM in browsers that can't record MP4).

**360° (`360.html`):** open stitched 360 photos and videos (2:1 equirectangular) from Samsung Gear 360, Insta360, Ricoh Theta, GoPro MAX and phone panoramas. Raw dual-lens files, such as Samsung Gear 360 originals, are detected and stitched, with sliders to line up the seam. Level the horizon, set the starting direction, adjust colour, and switch between the 360 view, a little planet and a flat view. Save 360 photos with the metadata Facebook and Google Photos look for, a picture of what you see, a 360 video, or a flat video of one view. Insta360 .insv and GoPro .360 files must be exported from the camera's app first.

**3D (`3d.html`):** add cubes, spheres, cylinders, cones, rings and panels; open GLB, glTF, OBJ, STL and PLY models; move, rotate and resize with handles or exact numbers (in millimetres); snap to the grid; change colour and finish; undo and redo; export GLB (web, AR, Booth's shop), STL (3D printing), OBJ or a PNG picture.

3D and 360 use three.js r169 (MIT), included in `vendor/three/`.

## Updating your GitHub repo
Upload everything in this folder, keeping the folder structure: `index.html`, `video.html`, `360.html`, `3d.html`, `README.md`, the `assets` folder and the `vendor` folder. The new studios must be opened from your GitHub Pages address (or a local server), not by double-clicking, because browsers block their modules on `file://` pages.
