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
- **Save** as PNG, JPG, WebP (and AVIF where the browser supports it), choose quality and size, or keep the file under a limit such as 240 KB for online applications. Copy to clipboard or share on phones.
- Undo/redo (Ctrl+Z / Ctrl+Shift+Z), hold **Compare** to see the original, **Start over** anytime.

## Good to know
- **Background removal needs the internet the first time.** It downloads an AI model (tens of MB) from IMG.LY's servers; your browser caches it after that. The photo itself is processed on your device.
- The background-removal library (`@imgly/background-removal`) is licensed under **AGPL-3.0**. Free personal and non-commercial use is fine. If you ever turn Booth into a commercial product, review that licence or swap the library.
- Very large photos are reduced to 4096 px on the longest side for smooth editing.
- Passport rules differ by country and change. Always check the official requirements before you submit. Print sheets at 100% size, not "fit to page".
- iPhone HEIC photos open fine on iPhone/Safari. On other browsers, export them as JPG first.
