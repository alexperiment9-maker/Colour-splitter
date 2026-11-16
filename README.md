# Colour Splitter Pro

A colour grading tool in one web page, made for cinematographers, editors and colourists. Grade a frame, check it on scopes, and export the look as a `.cube` LUT for your editing app.

## Grading tools (all go into the LUT)

- **Input / Log** – Apple Log, Sony S-Log3, Panasonic V-Log, ARRI LogC3 → Rec.709 with a soft highlight roll-off
- **Light & white balance** – exposure in stops, temperature, tint, tap-a-grey-card white balance, auto white balance
- **Tone** – contrast with pivot, highlights, shadows, whites, blacks, auto tone
- **Curves** – master + red, green, blue
- **Colour wheels** – lift, gamma, gain, offset with level sliders
- **Colour (HSL)** – saturation, skin-safe vibrance, tap any colour to change its hue, saturation and lightness
- **Split tone** – shadow and highlight tint with balance
- **B&W & film** – fade / matte blacks, black & white with colour filters and channel mixer
- **Shot match** – load a reference frame and match colour and contrast to it
- **Looks** – 11 built-in looks, save your own, share looks as code

## Checking tools

- Histogram (with clipping %), waveform, RGB parade, vectorscope with skin-tone line
- ARRI-style false colour for exposure
- Split before/after, hold to see the original
- Undo / redo
- Colour breakdown of the graded frame: colour groups with shades and %, main colours with HEX, RGB, HSL, CMYK

## Export

`.cube` 3D LUT in 17, 33 or 65 size. Works in Premiere Pro, DaVinci Resolve, Final Cut Pro, CapCut, LumaFusion, Photoshop, OBS. The preview runs through the same LUT, so the file matches the screen.

Note: sharpening, grain and vignettes can't be stored in a LUT, so they aren't included.

Everything runs in your browser. Photos are never uploaded.

## Put it online with GitHub Pages (no coding)

1. Sign in to GitHub and click **New repository**. Name it `colour-splitter`, set it to **Public** and click **Create repository**.
2. On the new repo page, click **uploading an existing file**.
3. Drag in **all** the files from this folder and click **Commit changes**.
4. Go to **Settings → Pages**. Under **Branch**, choose `main` and `/ (root)`, then click **Save**.
5. After a minute or two it's live at `https://YOUR-USERNAME.github.io/colour-splitter/`.

**Install it:** open the link in Chrome on your phone → menu (⋮) → **Install app**. On a computer, click the install icon in the address bar. Once installed it works offline.

If you already uploaded the older version, just upload these files again and replace the old ones.
