# ACE Color Correction Implementation

This project implements the Automatic Color Equalization (ACE) algorithm for unsupervised image enhancement, based on the research paper "A new algorithm for unsupervised global and local color correction" by Daniele Marini, Alessandro Rizzi, and Carlo Gatta (2002). It was developed as part of the IMA201 course at Télécom Paris.

## Course Information

- **Course:** IMA201
- **Institution:** Télécom Paris
- **Date:** November 14, 2023
- **Supervisor:** Christophe Kervazo

## Project Team

- Adnane El Bouhali
- Nourelhouda klich

## Overview

ACE is an algorithm for automatic color correction in digital images. It's based on a computational model of human vision and combines two basic global equalization mechanisms: "White Patch" and "Gray World". The algorithm performs local filtering by considering the spatial color distribution in the image.

## Features

- Spatial chromatic adjustment
- Dynamic tone reproduction scaling
- Color constancy
- Brightness constancy and dynamic modification
- Contrast modification (both global and local)

## Implementation Details

The implementation includes:

1. Different r(·) functions:
   - Linear
   - Signum
   - Saturation

2. Various distance functions d(·):
   - Euclidean
   - Inverse exponential
   - Manhattan
   - Maximum

3. Two scaling methods for dynamic tone reproduction:
   - Linear scaling
   - Gray World White Patch scaling

## Results

The implementation successfully improves color correction in images, enhancing details and overall visual perception. It demonstrates effectiveness in:

- Adjusting brightness based on original image conditions
- Maintaining color consistency under different lighting conditions
- Modifying both global and local contrast

## Usage

This project is implemented as a Jupyter notebook. To use it:

1. Ensure you have Jupyter Notebook installed on your system.
2. Clone this repository to your local machine.
3. Navigate to the project directory.
4. Launch Jupyter Notebook
5. Open the notebook file (e.g., `ACE_implementation.ipynb`).
6. Run the cells in order to execute the ACE algorithm.

Note: The "content" folder in the project directory contains all the images used for testing and demonstration.

## Dependencies

Ensure you have the following Python libraries installed:

- numpy
- matplotlib
- scipy
- Pillow
- opencv-python

## Acknowledgements

We would like to thank our course supervisor, Christophe Kervazo, for his guidance throughout this project.

## References

1. Daniele Marini, Alessandro Rizzi, Carlo Gatta. "A new algorithm for unsupervised global and local color correction." (2002)
2. Pascal Getreuer. "A new algorithm for unsupervised global and local color correction." IPOL Journal, 2 (2012)