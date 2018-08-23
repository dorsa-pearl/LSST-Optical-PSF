# LSST-Optical-PSF
 The script measures the sensitivity of the LSST optics PSF to deviations in flatness of the focal plane.
Objective: We investigate the size and shape dependence of the LSST optical PSF on sensor height and incoming field angle. 
Background:
The LSST optical prescription brings parallel rays into nearly perfect focus through reflections & refractions with optical elements.
The small imperfections from perfect focus that remain produce the size and shape of the optics part of the PSF.
These imperfections vary with height of the focal plane and position on  the focal plane.
Methodology:
We use the open source raytracing software batoid (https://github.com/jmeyers314/batoid) to simulate the LSST optics PSF.
For a given incoming angle and focal plane height, a grid of parallel rays is propagated through the system to the focal plane, forming the spot diagrams shown in Fig 1.
We measure the PSF size and shape from the moments of the spots.
We use this fit formula to characterize the height dependence of the PSF size
