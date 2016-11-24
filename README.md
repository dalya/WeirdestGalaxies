# Outlier Detection Algorithm on Galaxy Spectra

This repository contains the basic outlier detection algorithm that we used to find the weirdest galaxies in the Sloan Digital Sky Survey (SDSS). 
We used unsupervised Random Forest (RF) algorithm to assign a similarity measure (or distance) between every pair of galaxy spectra in the SDSS. We then used the distance matrix to find the galaxies that have the largest distance, on average, from the rest of the galaxies in the sample, and defined them as outliers.

The repository contains an iPython notebook with step-by-step instructions to detect outliers on simulated, 2D, data. If you have trouble constructing your input data on which to perform outlier detection, please let us know (dalyabaron@gmail.com) and we will help!

## Authors
* Dalya Baron (TAU)
* Dovi Poznanski (TAU)

## Requirements
The code requires the following packages:
* Python 2.7
* numpy 1.11.1
* matplotlib 1.5.3
* scikit-learn 0.17.1
* (In the future: a development version of scikit-learn will be necessary to run some of the algorithms)

## Weirdest SDSS Galaxies
Additional information about the outlier detection algorithm and its implementation on SDSS galaxy spectra:
* Associated paper, MNRAS accepted: https://arxiv.org/abs/1611.07526
* The weirdness score of ~2.5M SDSS galaxies: http://wise-obs.tau.ac.il/cgi-bin/dovip/weird_galaxies.cgi. Here you can get the weirdness score of your favourite galaxy or use the *I'm feeling lucky* option to browse a random galaxy from the top 4000 weirdest galaxies.
* A short description about the algorithm: http://wise-obs.tau.ac.il/~dovip/weird-galaxies/about.html.

## Credits
Our work is based on the study by Shi & Horvath (2006), **Unsupervised Learning with Random Forest Predictors**, though with a few modifications that are necessary to optimaly detect outliers on galaxy spectra.
