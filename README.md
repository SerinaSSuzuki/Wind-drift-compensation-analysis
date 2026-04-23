# Wind-drift-compensation-analysis
This repository provides the full code for cleaning GPS data acquired from GiPSy, Axy-Trek, and Pinpoint VHF devices attached to seabirds, and for analyzing the data with a hierarchical Bayesian model to visualize age differences in wind drift compensation.
Code 1 is specific to our dataset's cleaning process and can be skipped if you are using your own dataset.

**Input files**
Two types of input files are required: a GPS file and an individual file. The individual file is available in the "Input" folder, which also contains a dummy GPS file illustrating the required format. The GPS file must be downloaded from the Biologging Intelligent Platform (BiP; https://www.bip-earth.com).

**HMM-based state classification**
A large number of approaches were tested in pursuit of better classification accuracy, resulting in highly complex code. This repository therefore provides only the foundational version. The code used in the manuscript was produced by first running this base code, then manually adjusting the parameters for each individual while inspecting the output figures until optimal classification was achieved. The GPS tracking plots generated from the final state classification are provided in the file: GPS tracking plot.

**Wind data**
This code contains two separate sections for adding wind data columns, but only one is actually needed (the other is retained for reference). For a detailed explanation of the wind-matching process, refer to Code 4. To run this section, you will need to download the required .nc files from ERA5 (https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels?tab=download) in advance.
