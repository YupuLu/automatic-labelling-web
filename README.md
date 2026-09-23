# Paper project page

This directory contains a static project page for **Automatic Labelling for Bimanual Mobile Manipulation**.

## Paper and authors

The page lists Yupu Lu and Jia Pan, School of Computing and Data Science,
The University of Hong Kong, HKSAR, following the manuscript's author block.
Paper links and the BibTeX citation point to <https://arxiv.org/abs/2609.24059>.
No local `paper.pdf` is needed.

Code / project and supplementary material are marked **TBR** (to be released).
When these resources are available, replace the disabled hero button and pending
resource rows with links in `index.html`.

## Directory layout

```text
automatic-labelling/
├── figures/       # Web figures, including the Galaxea and BEHAVIOR-1K examples
├── index.html
├── style.css
└── README.md
```

The method groups the arm and base/torso figures side by side, followed by the
full-width cross-stream figure, under Stage 1 (kinematic trajectory segmentation).
A shared full-width reasoning figure illustrates Stages 2 and 3: phase-localised
VL reasoning and within-stream semantic aggregation. On small screens, the
paired figures stack vertically.

The page uses only image assets for figures; no PDF viewer is required. Task
examples use native expandable panels, with floor-cloth wiping open initially.
Selecting a method or task-example figure opens its full-resolution image.

## Preview locally

From the root directory, run a local static server so that both
`web/` and its sibling `figures/` directory are available:

```bash
python3 -m http.server 8000 --bind 127.0.0.1
```

Then open <http://localhost:8000/>. 
The page requires no JavaScript or build step.

## Publishing

Copy the directory to a dedicated public repository,
preserving their sibling layout. With GitHub Pages serving that repository's
root, the page will be at `https://<username>.github.io/<repository>/`.
A personal homepage is optional.
