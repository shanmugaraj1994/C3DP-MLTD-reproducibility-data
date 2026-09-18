# Reproducibility Package for MLTD-Based Buildability Failure Prediction

## Overview

This repository contains representative image data, extracted
layer-thickness measurements, MLTD values, prediction parameters,
and pseudocode supporting the manuscript:

"Buildability Failure Prediction and Supervisory Decision-Support
in Concrete 3D Printing Using Image Data"

## Repository Contents

- `representative_images/`: Raw and processed images from stable
  and collapse-prone prints.
- `representative_data/`: MLTD data.
- `pseudocode/`: Pseudocode for the computer-vision and
  collapse-prediction workflows.
- `parameters/`: Final image-processing and prediction parameters.

## Method Summary

1. Extract one image after each layer deposition.
2. Isolate the printed element using U2-Net.
3. Detect inter-layer boundaries using Canny edge detection and
   the probabilistic Hough transform.
4. Measure layer thickness at 30 sampling positions.
5. Calculate layer deformation and MLTD.
6. Calculate overall and incremental MLTD slopes.
7. Apply the system-specific LBV and persistence criteria.

## Data Scope

The repository contains representative data from stable and
collapse-prone printing trials. The complete raw image dataset is
not deposited because of its large storage size but is available
from the corresponding author upon reasonable request.

## Software Dependencies

- Python
- OpenCV
- NumPy
- pandas
- Pillow
- U2-Net

## Citation

Please cite the associated journal article and archived Zenodo
release.

## Contact

other author: Shanmugaraj Senthilnathan
Indian Institute of Technology Madras