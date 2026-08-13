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
held-out specimen **RS315**. The GIFs below preview the held-out test
specimen; the three training-specimen reconstructions (RS307, RS330, RS615)
are available on the [live page](https://marcelab.caece.net/3D-results/).

| Specimen | Real | Generated |
|---|---|---|
| RS315 &nbsp;*(held-out test)* | ![real RS315](gifs/real_rs315.gif) | ![generated RS315](gifs/generate_rs315.gif) |

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


## License

Add a license file appropriate for your lab's data-sharing policy before
making this repository public (e.g. CC-BY-4.0 for the visualizations).
