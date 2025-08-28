# NONSD-Gait: A Multi-sensor Gait Dataset Collected Under Non-standardized Dual-Task Conditions

## About
This repository contains Python code for processing the dataset NONSD-Gait.
The publication about this dataset will soon be online.

The scripts achieves the following main functions:
* Segment the complete data recorded by the MOCAP, Kinect, and IMU sensors into straight-line and turning phases
* Extract kinematic parameters and spatiotemporal gait parameters from the three devices for each phase
* Perform differential analysis for single-task and dual-task conditions, and consistency analysis between devices


## Usage steps
(1) Clone repository
> https://github.com/Vanessa-lyy/Multi-source-gait-dataset.git

(2) Create environment with anaconda3

(3) Download dataset 
> https://doi.org/10.5061/dryad.2rbnzs7z3
 
(4) Modify the file path in the code

## Usage note
### Folder: Preprocessing
This folder contains two subfolders: **Raw_Processed** and **Processed_Parameters**.

* **Raw_Processed**: Interpolate and denoise the raw data, then segment it into straight-line and turning phases.

* **Processed_Parameters**: Extract kinematic parameters and spatiotemporal gait parameters from the three devices for each phase.

### Folder: Technical Validation
This folder contains two subfolders: **Data quality control**, **Difference between tasks** and **Consistency between MOCAP and Kinect**.

* **Data quality control**: Validate the effectiveness of timestamp segmentation and the consistency between two experiments.

* **Difference between tasks**: Test the differences in spatio-temporal gait parameters and kinematic parameters between single-task and dual-task conditions during straight-line and turning phases.

* **Consistency between MOCAP and Kinect**: Investigat the consistency of spatio-temporal gait parameters between MoCap and Kinect.

Specific research details can be referred to the published article for details: https://www.nature.com/articles/s41597-025-05458-y#MOESM1
