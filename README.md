# Udacity's Self-Driving Car Engineer Nanodegree, Term 2, Project 3 - Particle Filter (Localization)


#### Remarks
Modified files: 
1. `particle_filter.cpp`
2. `particle_filter.h`:
* added `ObservationPackage` struct to track landmark data
* declared additional function `LandmarkObs transformObservation(Particle& particle, LandmarkObs& observation);`
to transform coordinates
* declared additional function `ObsevationPackage closestLandmarkLocation(LandmarkObs &obs, Map map_landmarks, 
double thershold);` to obtain closest landmark data
3. `helper_functions.h` (added Multivariate Gaussian probabilty calculation)

To build and run:
```bash
build.sh
run.sh
```


