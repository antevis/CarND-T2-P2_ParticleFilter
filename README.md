# Udacity's Self-Driving Car Engineer Nanodegree, Term 2, Project 3 - Particle Filter (Localization)


#### Remarks
Modified files: 
1. `particle_filter.cpp`, obviously.
2. `particle_filter.h`:
* added `ObservationPackage` struct to track landmark data
* declared additional function `transformObservation()`
* declared additional function `closestLandmarkLocation()`
* changed the return type and signature of `SetAssociations()` function so that it modifies the existing `Particle` instance 
associations and transformed observations instead of generating a new `Particle`.
* removed `weights` variable. When resampling, dynamically extract weights from the `Particles`'c vector directly. 
3. `helper_functions.h`
* added `multivariateGaussProb()`, `sigmoidalDiff()` functions to compute multivariate Gaussian probability calculation.
The latter is just a helper for the former.

To build and run:
```bash
build.sh
run.sh
```


