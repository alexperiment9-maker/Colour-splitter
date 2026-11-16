# Colour Splitter

A one-page web app that breaks a photo into its colours, lets you recolour any of them, and exports the look as a `.cube` LUT.

## Features

- **Take a photo or pick an image** (drag and drop works on a computer)
- **Colour groups** – Red, Orange, Yellow, Green, Cyan, Blue, Purple, Pink, Brown, White, Grey, Black, with the % of the picture each covers
- **Shades per colour (1–8)** – splits every group into lighter and darker shades, each with its own %
- **Main colours** – the biggest colours in the picture with their name, HEX, RGB, HSL, CMYK and brightness
- **Edit colours** – tap any colour on the photo to change its hue, saturation and lightness, and set how wide a range of similar colours it affects
- **Whole-picture controls** – exposure, contrast, saturation, warmth, tint
- **Quick looks** – Teal & orange, Warm film, Moody, Vivid, Black & white
- **Hold "before"** to compare with the original
- **Export a .cube LUT** (17, 33 or 65 size) for Premiere Pro, DaVinci Resolve, Final Cut, CapCut, Photoshop, LumaFusion and more

Everything runs in your browser. Photos are never uploaded anywhere.

## Put it online with GitHub Pages (no coding)

1. Sign in to GitHub and click **New repository**. Name it `colour-splitter`, set it to **Public** and click **Create repository**.
2. On the new repo page, click **uploading an existing file**.
3. Drag in **all** the files from this folder (`index.html`, `manifest.json`, `sw.js`, the icon PNGs, `README.md`, `LICENSE`) and click **Commit changes**.
4. Go to **Settings → Pages**. Under **Branch**, choose `main` and `/ (root)`, then click **Save**.
5. After a minute or two the app is live at `https://YOUR-USERNAME.github.io/colour-splitter/`.

**Install it:** open the link in Chrome on your phone → menu (⋮) → **Install app**. On a computer, click the install icon in the address bar. Once installed it works offline too.

## How the LUT works

The preview runs your photo through the same 3D LUT that gets exported, so the .cube file gives the same result as the screen. Colour edits are matched by hue (or by lightness for whites, greys and blacks) with a soft falloff, so the edits blend smoothly.
