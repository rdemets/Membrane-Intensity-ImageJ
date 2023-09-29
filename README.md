# Motivations


The aim of this macro is to measure the intensity of individual cells in a monolayer using Cellpose to segment the cells in Fiji

## How to install

To install, drop the file in `Fiji.app>macros>toolsets` folder. Restart Fiji and the macro name will then appear under the **>>** menu on the right hand side of Fiji bar.

## Requirements

This macro requires **PTBIOP** from the Fiji plugins updater. Please follow the instructions from their [website](https://github.com/MouseLand/cellpose) to install Cellpose GUI and cite the respective authors.

## How to use

To activate the macro, find it under the **>>** menu on the right hand side of Fiji bar. Two buttons should appear on the Fiji bar. 
Three buttons will appear, the first one doing the segmentation using Cellpose. It takes as an input a folder with all the CZI files, and gives the rois as output. The macro will ask which channel correspond to the membrane staining, which one is the nuclei staining.
<br>The second button will load back the ROI files and do the rings depending on the thickness entered. So far, it is making a band by shrinking the rois. The program is making the assumptions that all images are the same size within the batch of images.
<br>The third button is just to do the measurement of those rings for all channels. The output will be a csv file containing the results.



## Citations

Please cite [Cellpose](https://www.nature.com/articles/s41592-020-01018-x) if you use this macro.

## Updates history
(0.0.1) Segment using Cellpose for individual cells
<br>(0.1.0) Add Dialog box
<br>(0.1.1) Tasks splitted into three buttons
<br>(0.1.2) Add size filter for cell detections