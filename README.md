# Winfree Oscillatory Neural Network Project Page

This repository hosts the project page for **Winfree Oscillatory Neural Network (WONN)**.

WONN is a dynamical neural architecture based on generalized Winfree synchronization dynamics. It represents neural states as phase variables on the toroidal phase space \((S^1)^d\), and evolves them through structured oscillatory interactions for image recognition and reasoning tasks.

**Project page:** <https://jiawen-dai.github.io/WONN_Project_Page/>  
**Code:** <https://github.com/Jiawen-Dai/WONN>

> This repository contains only the static website. The model implementation and training scripts are maintained in the code repository above.

## Contents

The page provides a compact overview of the paper, including:

- the connection from classical Winfree dynamics to WONN;
- the WONN architecture and its hierarchical sensitivity--influence interaction mechanism;
- image classification results on CIFAR and ImageNet;
- reasoning results on Maze-hard and Sudoku;
- qualitative visualizations of Maze-hard path formation, phase-mode dynamics, and interaction-energy diagnostics.

## Repository Structure

```text
.
├── index.html              # Main project page
├── static/images/          # Figures, tables, GIFs, and visualizations used by the page
├── assets/                 # Template styles, scripts, fonts, and other static assets
├── clarity/                # Clarity template CSS/JS files
├── clarity.html            # Original/reference Clarity template page
├── LICENSE
└── README.md
```

The page is static and can be hosted directly with GitHub Pages.

## Local Preview

Open `index.html` directly in a browser, or serve the directory locally:

```bash
python3 -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## Updating the Page

Most content edits should be made in `index.html`.

Common updates include:

- updating the paper link in the `Paper` button;
- updating the code link in the `Code` button;
- replacing or adding figures under `static/images/`;
- updating experimental tables;
- updating the BibTeX entry in the `#bibtex` section.

The current page uses MathJax for equations and local static images for the main visual assets.

## Deployment Notes

For GitHub Pages, keep `.nojekyll` in the root directory so that static files and folders are served without Jekyll processing.

Before committing, remove local macOS metadata files if they appear:

```bash
find . -name ".DS_Store" -delete
rm -rf __MACOSX
```

## Acknowledgements

This website is built on the [Clarity Template](https://shikun.io/projects/clarity), originally designed by Shikun Liu, and incorporates elements from the [Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template).

## License

The template-derived website code follows the Creative Commons Attribution-ShareAlike 4.0 International License. Please keep the footer attribution when reusing or adapting the page.
