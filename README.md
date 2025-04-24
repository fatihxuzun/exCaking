# exCaking for Polycrystal Diffraction Strain Analysis
![logo](https://raw.githubusercontent.com/fatihxuzun/exCaking/main/exCaking_logo.png)

## Dependencies
* MATLAB R2022a

## Installation
Download 'calibration.p', 'reference.p' and 'analyse.p' to your project folder.

/myProjectFolder$

## exCaking Command Line
calibration(peak_range, set_brightness, sub_pixel, file_format)

* peak_range - Pixelwise ring peak fitting range of calibration file
* set_brightness - Brightness of calibration file ranging from 0.0 to 1.0
* sub_pixel - Step size for sub-pixel level analysis of calibration file
* file_format - File format of calibration file

reference(peak_range, set_brightness, sub_pixel, file_format)

* peak_range - Pixelwise ring peak fitting range of polycrystal diffraction data
* set_brightness - Brightness of reference file ranging from 0.0 to 1.0
* sub_pixel - Step size for sub-pixel level analysis of polycrystal diffraction data
* file_format - File format of polycrystal diffraction data

analyse(n_of_workers, ang_step_size)

* n_of_workers - Number of parallel processes
* ang_step_size - Angular step size within the range of 360 degrees

## exCaking Input Files
Follow the instructions from command window.

## Usage
The guide for analysing polycrystal diffraction data:

https://github.com/fatihxuzun/exCaking/blob/main/tutorial.pdf

## Outputs
/myProjectFolder/dStore$

* circle_calibration.mat
* circle_calibration_selected_points.png
* circle_calibration_fit_line.png
* circle_calibration_fit_peaks_start.png
* circle_calibration_fit_peaks_end.png

* multipeak_reference.mat
* multipeak_reference.png
* multipeak_reference_peaks_start.png
* multipeak_reference_peaks_end.png

* myDataFolder_exCaking.csv

## Scientific Usage
The exCaking console application was developed to improve strain analysis in polycrystalline materials by offering a more accurate approach to processing diffraction data from Debye-Scherrer rings, enhancing the precision of elastic strain measurements. Please cite:

Uzun, F.; Daisenberger, D.; Liogas, K.; Wang, Z.I.; Chen, J.; Besnard, C.; Korsunsky, A.M. Extended Caking Method for Strain Analysis of Polycrystalline Diffraction Debye–Scherrer Rings. Crystals (2024). https://doi.org/10.3390/cryst14080716

## Publications
Uzun, F., Slim, M.F., Basoalto, H. et al. Application of strain tomography and contour method to residual stress analysis in additively manufactured CM247LC superalloy parts. Prog Addit Manuf (2025). https://doi.org/10.1007/s40964-025-01116-2
