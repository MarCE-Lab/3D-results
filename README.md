# 3D Damage Visualization — RC Bridge Columns (GRAF)

Supplementary material for:

> **3D Damage Prediction for RC Bridge Columns via Physics-Informed Generative Radiance Fields**
> Chia-Yu Chou, Rih-Teng Wu
> Department of Civil Engineering, National Taiwan University
> Submitted to *Engineering Structures*

This repository hosts 360° rotating visualizations of real vs. GRAF-generated
RC bridge column damage that could not be included as static figures in the
manuscript (PDF does not support embedded video/GIF).

## Live page

The full interactive gallery (higher-quality MP4, side-by-side layout) is
live at:

```
https://marcelab.caece.net/3D-results/
```

The animated previews below are lower-resolution GIFs for quick viewing
directly on GitHub; see the live page above for full quality.

## Preview

**Fold 2** configuration — trained on RS307, RS330, RS615; evaluated on
held-out specimen **RS315**.

| Specimen | Real | Generated |
|---|---|---|
| RS315 &nbsp;*(held-out test)* | ![real RS315](gifs/real_rs315.gif) | ![generated RS315](gifs/generate_rs315.gif) |
| RS307 &nbsp;*(training)* | ![real RS307](gifs/real_rs307.gif) | ![generated RS307](gifs/generate_rs307.gif) |
| RS330 &nbsp;*(training)* | ![real RS330](gifs/real_rs330.gif) | ![generated RS330](gifs/generate_rs330.gif) |
| RS615 &nbsp;*(training)* | ![real RS615](gifs/real_rs615.gif) | ![generated RS615](gifs/generate_rs615.gif) |

## Contents

- `index.html` — visualization gallery (real vs. generated, 360° rotation)
- `assets/` — MP4 videos (256×256, 25 fps, 72 frames covering 0°–360°)
  - `real_rsXXX.mp4` — real captured multi-view rendering
  - `generate_rsXXX.mp4` — GRAF-generated result under the corresponding
    specimen's structural condition
- `gifs/` — downsampled GIF previews (160 px, 12 fps) for embedding in this
  README

The videos shown correspond to the **Fold 2** cross-validation configuration
(trained on RS307, RS330, RS615; evaluated on held-out specimen RS315), as
defined in Table 5 of the manuscript.

## Enabling GitHub Pages

1. Push this repository to your lab's GitHub organization.
2. Go to **Settings → Pages**.
3. Under **Source**, select the `main` branch and `/ (root)` folder.
4. Save. The page will be live at the URL shown above within a few minutes.

## Recommended: archive with Zenodo for a persistent DOI

GitHub links can break if a repo is renamed, moved, or deleted. To ensure the
supplementary material remains citable long-term:

1. Connect this repository to [Zenodo](https://zenodo.org/) via
   GitHub → Zenodo integration (one-time setup).
2. Create a GitHub **Release** for this repo — Zenodo will automatically
   archive it and mint a DOI.
3. Use the DOI link (e.g. `https://doi.org/10.5281/zenodo.XXXXXXX`) in the
   paper's Data Availability statement instead of (or in addition to) the raw
   GitHub Pages URL.

## License

Add a license file appropriate for your lab's data-sharing policy before
making this repository public (e.g. CC-BY-4.0 for the visualizations).
