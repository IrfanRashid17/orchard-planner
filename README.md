# Orchard Planner

Plan high-density (HD) and ultra-high-density (UHD) apple orchards in the browser. Enter a plot, and the planner draws a to-scale layout with every tree, trellis pole, anchor and hail-net cross wire, counts them, and gives you a row-by-row table for marking out in the field.

It is a single `index.html` file with no build step and no server.

## Features

- **Three ways to enter land**
  - *Ready-made shapes*: rectangle, four-sided plot (bottom, left, right and top), block with a strip, rounded corner.
  - *Walk the boundary*: enter each side's length and direction (N, NE, E… or any bearing); curved sides by how far they bulge.
  - *Draw on a grid*: click to add corners, drag to move them (snaps to 0.5 ft), or type exact positions.
- **Layout rules you control**: row and plant spacing, side gap, tiller gap at the far end, gap at the start end, anchors at both ends / one end / none, anchor-to-end-pole distance, optional tree in the anchor gap, maximum pole spacing.
- **Quick presets**: M9 UHD 9 × 3.25 ft, M9 UHD 10 × 3 ft, MM111 HD 10 × 8 ft, MM111 HD 8 × 8 ft.
- **Poles for hail nets**: middle poles always sit centred between two trees, evenly spaced, and line up across all rows so cross wires run straight.
- **Best row direction**: tries rows up-and-down, across and along every straight side, shows the tree count for each, and picks the best (you can choose another).
- **Results**: trees, rows, poles, anchors, area (sq ft and kanal, 1 kanal = 5,445 sq ft), trees per kanal, trellis wire length.
- **Exports**: PDF (drawing plus marking-out table), SVG and CSV.
- **Saved plots**: kept in your browser; export and import them as a JSON file to move between devices.

## Use it

Open `index.html` in any modern browser, or use the GitHub Pages link once it is published (see below).

PDF export loads [jsPDF](https://github.com/parallax/jsPDF) and [jsPDF-AutoTable](https://github.com/simonbengtsson/jsPDF-AutoTable) from the jsDelivr CDN the first time you click **Download PDF**, so that button needs an internet connection. Everything else works offline.

## Publish on GitHub Pages

1. Create a new repository on GitHub (for example `orchard-planner`).
2. Upload `index.html`, `README.md`, `LICENSE` and `.nojekyll` to the repository root.
3. In the repository, open **Settings → Pages**, set **Source** to *Deploy from a branch*, choose the `main` branch and the `/ (root)` folder, and save.
4. After a minute the site is live at `https://<your-username>.github.io/orchard-planner/`.

## Measurements

All distances are in feet. Row offsets in the table are measured from the plot edge the rows run along; positions along each row are measured from where the row meets the boundary at its start (anchor) end.

## License

Copyright © 2026 Irfan Rashid. All rights reserved. The source code may not be copied, modified or redistributed without written permission. See [LICENSE](LICENSE).
