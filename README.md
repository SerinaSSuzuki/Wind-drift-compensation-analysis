# Wind-drift-compensation-analysis
Full code for cleaning GPS data acquired from GiPSy, Axy-Trek, and Pinpoint VHF attached to seabirds and analyzing it with a hierarchical Bayesian model to visualize age differences in wind drift compensation

There are two types of input files: a GPS file and an individual file. The individual file is available on GitHub, while the GPS file must be downloaded from the Biologging Intelligent Platform (BiP; https://www.bip-earth.com).

For HMM-based state classification, a large number of approaches were tested
in pursuit of better classification accuracy, and the resulting code is
highly complex. This section therefore provides only the foundational version.
The code actually used in the manuscript was produced by first running this
base code, then manually adjusting the parameters for each individual while
inspecting the output figures, until the optimal classification was achieved.
The GPS tracking plots generated from the final state classification are
provided in the file: GPS tracking plot.
