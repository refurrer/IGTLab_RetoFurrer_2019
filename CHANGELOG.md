# Change Log
Project:  Topology analysis of polymer tube sections using microCT images<br/>
Author:   Reto Furrer<br/>
File(s):  IGTLab_RetoFurrer_2019<br/>

## V1 (2019-09-03, 44a5b58)
* Initial Version with basic functionallity
* Outer diameter detection of polymer tube
* Inner diameter cannot be detected (!)
* Based on canny edge detection

## V2 (2019-09-03, 29a69b9)
* Optimized inner diameter detection, e.g. masking
* Output of different images for visual checks
* Based on canny edge detection

## V3 (2019-09-04, 1409834)
* Added sobel filter
* Read Radius of edges manually

## V4 (2019-09-04, 3ca9af8)
* Removed sobel filter and replaced with canny edge detector
* Iteration over the whole circle coordinates added
* Code prepared for migration into function file

## V5 (2019-09-05, 06a5801)
* Methods moved to `utils.py` file. `IGTLab_RetoFurrer.ipynd` only work in conjunction with utils.py file from now
* Added for loop to iterate over the whole sample images for both samples
* Added multiple modes for the image masking `square`, `circle`and `ellipse`.
* Added multiple function for Filtering `gauss_filter()`and `median_filter()`.
* Funtion `inver_image()` part of `utils.py` file but unused.
* Not completed function `find_radii()` in `utils.py` file
* Added summary report function `print_summary()`.
* Added `export_results()` function to wrtie results into `.txt` file.
* Added `create_directories()` function to create proper invironment to file new images, graphics and text files.
* Added Description and comments to the code for further use of the program

## V6 (2019-09-05, 1ece74f)
* Completed function `find_radii()` to calculate the radii around the found edges.
* Only `utils.py`file changed

## V7 (2019-09-06, 1a03e11)
* Added 3D plot for wall thickness to emphazise with the idea of a topology
* Funtion `find_radii()` commented out. 
