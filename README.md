# Wind-drift-compensation-analysis
Full code for cleaning GPS data acquired from GiPSy, Axy-Trek, and Pinpoint VHF attached to seabirds and analyzing it with a hierarchical Bayesian model to visualize age differences in wind drift compensation

Code1 is only for cleaing our dataset, so you can skip it when you are using your dataset.

There are two types of input files: a GPS file and an individual file. The individual file is available on "Input" file, while the GPS file must be downloaded from the Biologging Intelligent Platform (BiP; https://www.bip-earth.com).　
A dummy GPS dataset (with fictional lon/lat values fitted to the actual data structure) can be obtained from the GPS folder. By formatting your data to match this structure, the code can be executed correctly. Skip Code1 if you are using this dataset.

For HMM-based state classification, a large number of approaches were tested
in pursuit of better classification accuracy, and the resulting code is
highly complex. This section therefore provides only the foundational version.
The code actually used in the manuscript was produced by first running this
base code, then manually adjusting the parameters for each individual while
inspecting the output figures, until the optimal classification was achieved.
The GPS tracking plots generated from the final state classification are
provided in the file: GPS tracking plot.

This code contains two separate sections for adding wind data columns, but only one of them actually needed (I left it for recording purpose). For a detailed explanation of the wind matching process, refer to code 4.
