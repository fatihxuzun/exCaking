# exCaking for Polycrystal Diffraction Strain Analysis
![logo](https://raw.githubusercontent.com/fatihxuzun/exCaking/main/exCaking_logo.png)

## Dependencies
* MATLAB R2022a

## Installation
Download 'calibration.p', 'reference.p' and 'analyse.p' to your project folder.

/myProjectFolder$

## exCaking Command Line
calibration(peak_range, set_brightness, sub_pixel, file_format)

* peak_range - Pixelwise ring peak fitting range in calibration file
* set_brightness - Brightness of calibration file ranging from 0.0 to 1.0
* sub_pixel - Step size for sub-pixel level analysis of calibration file
* file_format - File format of calibration file

reference(peak_range, set_brightness, sub_pixel, file_format)

* peak_range - Pixelwise ring peak fitting range of reference file
* set_brightness - Brightness of reference file ranging from 0.0 to 1.0
* sub_pixel - Step size for sub-pixel level analysis of reference file
* file_format - File format of reference file

analyse(n_of_workers, ang_step_size)

* n_of_workers - Number of parallel processes
* ang_step_size - Angular step size within the range of 360 degrees

## exCaking Input Files
Follow the instructions from command window.

## Usage
The guide for analysing training data:

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
Please cite:

doi link to the paper
