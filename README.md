# Outlier Detection Algorithm on Galaxy Spectra

This reporisoty contains the basic outlier detection algorithm that we use to find the weirdest galaxies in the Sloan Digital Sky Survey (SDSS). 
We use unsupervised Random Forest (RF) algorithm to assign a similarity measure (or distance) between every pair of galaxy spectra in the SDSS. We then use the distance matrix to find the galaxies that have the largest distance, on average, from the rest of the galaxies in the sample, and define them as outliers.

## Authours
* Dalya Baron (TAU)
* Dovi Poznanski (TAU)

## Requirements
The code requires the following packages:
* Python 2.7
* numpy 1.11.1
* matplotlib 1.5.3
* scikit-learn 0.17.1
* (In the future: a developnemt version of scikit-learn will be necessary to run some of the algorithms)

## Weirdest SDSS Galaxies
Additional information about the outlier detection algorithm and its implementation on SDSS galaxy spectra can be found at:
* Associated paper in MNRAS: (insert link here)
* The weirdness score of ~2.5M SDSS galaxies can be found here: http://wise-obs.tau.ac.il/cgi-bin/dovip/weird_galaxies.cgi
* Additional information about the algorithm can be found here:
..* Short description in our webpage: http://wise-obs.tau.ac.il/~dovip/weird-galaxies/about.html
..* See work by Shi & Horvath (2006): **Unsupervised Learning with Random Forest Predictors**.

