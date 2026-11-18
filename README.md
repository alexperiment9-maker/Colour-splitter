# Colour Splitter Pro

A colour grading tool in one web page, made for cinematographers, editors and colourists. Grade a frame, check it on scopes, and export the look as a `.cube` LUT for your editing app.

## Grading tools (all go into the LUT)

- **Input / Log** – Apple Log, Sony S-Log3, Panasonic V-Log, ARRI LogC3 → Rec.709 with a soft highlight roll-off
- **Light & white balance** – exposure in stops, temperature, tint, tap-a-grey-card white balance, auto white balance
- **Tone** – contrast with pivot, highlights, shadows, whites, blacks, auto tone
- **Curves** – master + red, green, blue
- **Primaries** – lift, gamma, gain, offset with master, red, green, blue controls
- **Colour (HSL)** – saturation, skin-safe vibrance, tap any colour to change its hue, saturation and lightness
- **Split tone** – shadow and highlight tint with balance
- **B&W & film** – fade / matte blacks, black & white with colour filters and channel mixer
- **Decode ref** – load any reference frame and it is rebuilt as normal sliders (exposure, contrast, blacks, whites, saturation, warmth, split tones) with a plain-English list of what makes the look, plus match % before/after. Quick one-knob match also available
- **Looks** – 11 built-in looks, save your own, share looks as code

## Keyboard (desktop)

`1`–`0` tools · `K` LUT check · `E` export · `N` film grain · `L` live camera · `R` record (live) · `P` peaking · `G` grid · `Space` play/pause (live: freeze) · `,` `.` frame step · `M` mark shot · `Z` undo · `Y` redo · hold `B` before · `S` split · `F` false colour · `W` pick neutral · `Esc` cancel

Every control has a number box for exact values and a ↺ reset.

## Live monitor (pocket field monitor)

Tap **Live** to use your phone or laptop camera as a grading monitor:
- your grade/LUT applied live
- false colour, zebras (90/95/100 IRE), focus peaking
- frame guides (2.39, 1.85, 16:9, 4:5, 9:16, 1:1) and rule-of-thirds grid
- live scope and exposure readout (average IRE, clipped %, crushed %)
- flip camera, full screen, screen stays awake
- **Freeze & grade**: grab the frame at full camera resolution to fine-tune and export the LUT

Needs the GitHub (https) version; the Claude viewer blocks camera access.

## Film grain

Amount, size, roughness, colour grain; presets 35mm, 16mm, Super 8. Scales with the frame, sits in the mid-tones, moves every frame. Added to saved images and videos (a LUT can't store grain).

## Video

Open an MP4/WebM clip and play it with the grade live. Scrub, step frame by frame, mark shots to jump between them, and export any frame at full resolution.

**Export graded video**: grade + grain + original sound, 720p / 1080p / original (up to 4K), rendered on the GPU in real time. Saves MP4 (H.264) where the browser supports it, otherwise WebM. Live camera has **● Rec** to record the graded view (with mic if allowed). Scopes and frame report update when paused. (ProRes/RAW and some HEVC files can't play in browsers: export an H.264 proxy.)

## LUT check

Tests your grade or any imported `.cube` and scores it /100: clipping, tone reversals, banding, flattened tones, grey tint, skin hue and saturation (skin types I–VI incl. wheatish and dusky Indian tones), colour shifts, black/white points, LUT size, out-of-range values. Imported LUTs can also be used on the frame with a strength slider.

**Auto-fix**: protect skin, soften clipping, smooth banding, optional neutral greys. Shows score before → after; use the fixed LUT on the frame or save it as a new .cube.

## Checking tools

- Histogram (with clipping %), waveform, RGB parade, vectorscope with skin-tone line
- ARRI-style false colour for exposure
- Split before/after, hold to see the original
- Undo / redo
- Colour breakdown of the graded frame: colour groups with shades and %, main colours with HEX, RGB, HSL, CMYK

## Export

- Graded image at full resolution (up to 6000 px), JPG or PNG
- Choose a LUT folder and an image folder once (Chrome/Edge on a computer); remembered next time, never overwrites
- Phones/Safari: saves to Downloads


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
