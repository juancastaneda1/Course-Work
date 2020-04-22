# Course-Work
A collection of small assignments from my undergraduate, most of which focus on a specific technique/topic

## Computer Generated Melodies Project
The purpose of this project was to create computer generated melodies over a sequence of musical chords (given as sound files, not chord names), with varying degrees of "pleasantness".

To accomplish this, the audio file of each chord was analyzed using a fast fourier transform in order to determine the notes being played, and from there get the name of the chord. Once the chord was identified, a series of musical notes was generated in such a way as to have a high or low degree of "pleasantness"

This was done by finding the major scale that corresponded to the chord that was identified. Each note was then generated at random, and if it was in the scale, automatically accepted. If not, the circle of fifths was used to estimate how dissonant the note would sound with respect to the major scale and ranked as "worst", "bad", or "better". A probability of acceptance was hardcoded for each ranking. These probabilities were modified several times in order to accept the dissonant notes none of the time, some of the time, or all of the time, in order to judge the "pleasantness" of the resulting melodies.

At the end of the code, some plots of superpositions of sinusoidal functions are generated in order to discuss consonance and dissonance.

Note: some of the helper functions were written by my partner for this assignment


## Time Series Analysis Labs

### Castaneda_Juan_Lab1.ipynb
Convolution, RL circuit response, smoothing seismogram data

### Castaneda_Juan_Lab2.ipynb
Fast Fourier transform, window functions, radial distribution function of liquid argon

### Castaneda_Juan_Lab3.ipynb
Notch filter, implementing notch filter as a rational filter, detrending and filtering atmospheric CO2 data.

### Castaneda_Juan_Lab4.ipynb
Cross-correlation of earthquake data and identifying normal modes of the Earth's internal structures


## Image understanding

### Seam carving and Harris corner detector.ipynb
As the name implies. Seam carving to remove columns from an image, as well as an implementation of a corner detection method.

### Image upscaling.ipynb
Increase the size of an image using convolution.

### Stitch_Images.ipynb
Stitch two images horizontally by matching keypints and using RANSAC to find an affine transformation for stitching the images together. Repeated again using a homography instead.

### Basic Road Anallysis for self-driving car.ipynb
Calculates depth given disparity matrix and camera parameters, calculate 3D position of objects, and a poor attempt at segmentation

### Homography.ipynb
Attempt at using a homography to calculate the dimensions of a door, given an image of a piece of paper taped to the door and the dimensions of the paper.

### Affine Transformation.ipynb
Visualize keypoints, match keypoints between images to apply an affine transformation to map a reference image to its location in the second image.

### A1_code.ipynb
Convolution, cross-correlation, and template matching


## Computational Physics Practicals

### Practical5.ipynb
Numerical integration, plane wave diffraction, determining the Stefan-Boltzmann constant, diffraction grating intensity patterns

### Practical 7.ipynb
Molecular dynamics analysis for protein folding

### Practical8.ipynb
Brownian motion, simulating radioactive decay

### Practical9.ipynb
Principal component analysis of protein folding simulation


## Double Square Well Correlation Diagram.ipynb
Solving the transcendental eigenvalue equation for a single fermion in a double square well potential to plot the energyy eigenvalues as a function of well separation
