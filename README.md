# 2025_epe_eeg
Behavioral data and analysis script for "Separable neural signals for reward and emotion prediction errors". 

The manuscript is published in Nature Communications at the following [doi to add]() and references an associated Zenodo [![DOI](https://zenodo.org/badge/1008435234.svg)](https://doi.org/10.5281/zenodo.15739721). 

# Setup
Clone repository or simply download in a zip file. 

The R Markdown file in the Analysis folder contains all the analysis code for main manuscript results. In order to run the code you'll need the following packages up-to-date:

```
library(tidyverse)       # tidy functions
library(here)            # relative paths
library(janitor)         # clean data types
library(R.matlab)        # read mat files
library(lme4)            # mixed-effects regression
library(lmerTest)        # mixed-effects regressions
library(marginaleffects) # marginal effects for regressions
library(AICcmodavg)      # predictSE()
library(car)             # VIF()
library(sjPlot)          # tab_model()
library(viridis)         # color scheme
library(cowplot)         # plot_grid()
library(styler)          # graph styles
library(rmcorr)          # repeated measures correlation 
library(rstatix)         # cohen's d
library(effectsize)      # cohen's d
```

# Folders
This repo contains the following folders: analysis, data, and graphs. 

1. **analysis**

   Main analysis script can be found here showing results and code in order of presentation in the manuscript.

2. **data**

   Cleaned behavioral and ERP data can be found here. Continuous artifact-cleaned EEG data per participant can be found in an associated [OSF repository](https://osf.io/ap4x7/). These files are compatible with [EEGLAB](https://sccn.ucsd.edu/eeglab/).

3. **graphs**

   Graphs produced for manuscript from R. Note that some style changes have been added to the final graphs in the manuscript using Adobe Illustrator. 

# Contact
If you have any questions or suggestions please feel free to open an issue on this repo or email me directly at joseph.p.heffner@gmail.com.

