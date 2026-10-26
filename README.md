
# Roman Microlensing Data Challenge (2026)

**Exploratory analysis of simulated microlensing observations for NASA's Nancy Grace Roman Space Telescope.**

**Challenge:** RGES-PIT Roman Microlensing Data Challenge (Beginner tier)  
**Status:** In progress  
**Language:** Python

## Overview

This repository documents my work on the **2026 Roman Microlensing Data Challenge**, organized by the [Roman Galactic Exoplanet Survey Project Infrastructure Team (RGES-PIT)](https://rges-pit.org/data-challenge/).

I'm using simulated Roman-like photometric data to investigate the shapes of gravitational microlensing light curves, identify unusual candidate events, and develop a workflow for testing lens models against observations.

**The data are simulated:** this project does not report detections made by the Roman Space Telescope.

## What I've worked on

- Loaded and explored a dataset containing **9,230,048 photometric observations across 188 targets**.
- Separated measurements by the **F087, F146, and F213 filters**.
- Plotted **magnitude versus time** with photometric error bars and examined data-quality information, including saturation flags.
- Inspected event light curves for features such as unusual brightening, dimming, multiple peaks, and possible caustic signatures.
- Flagged and organized **preliminary candidates** for closer analysis.

These visual classifications are **not confirmed planetary detections** or final lens classifications.

## Data and tools

**Dataset:** [RGES-PIT Beginner dataset on Hugging Face](https://huggingface.co/datasets/RGES-PIT/Beginner)  
**Tools:** Python, Jupyter Notebook, pandas, NumPy, Matplotlib, PyArrow, and `huggingface_hub`.

The analysis uses observation times, measured magnitudes, magnitude uncertainties, filter information, and quality flags from the simulated dataset.

## Notebook

**[Open the analysis notebook](./Roman%20Microlensing%20Data%20Challenge%202026.ipynb)**

To run the notebook locally or in Google Colab:

1. Open the linked `.ipynb` file in Jupyter Notebook or Google Colab.
2. Install any missing packages:

   ```bash
   pip install pandas numpy matplotlib pyarrow huggingface_hub
   ```

3. Run the cells in order. An internet connection is needed for the notebook to retrieve the dataset from Hugging Face.

## Next steps

- Refine the preliminary candidate classifications.
- Fit basic **single-lens microlensing models** and examine residuals.
- Investigate whether selected unusual events require more complex lens models.

**Project status:** Exploratory analysis and candidate screening are underway; validated model-fitting results are not yet included here.

## Acknowledgments

The challenge and simulated data are provided by **RGES-PIT**. This repository documents my own analysis of the challenge dataset and is **not an official NASA or RGES-PIT project**.
