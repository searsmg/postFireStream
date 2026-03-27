# Geographic variability in stream responses to wildfire

This repository contains data processing scripts, analysis code, and supporting materials for a study examining post-fire stream responses to rainfall in northern Colorado.

## Overview

This study evaluates how stream responses to rainfall vary:

- Between fires on the **east and west side of the Colorado Front Range**
- Between **snow zones (intermittent vs. seasonal)**
- Across **years following fire disturbance**

The analysis focuses on two major wildfires:

- Cameron Peak Fire  
- East Troublesome Fire  

## Scripts in this repo
- **extractCatchmentVars** is used to extract catchment-level dNBR, contributing area, snow persistence, potential water deficit, soil characteristics, slope, etc.
- **extractWhiteboxVars** uses the whitebox package to determine elongation ratio, geomorphons, flow accumulation, recharge areas, hypsometric analyses, flowpath length, etc.
- **catchmentVarsPCA** runs a PCA on the catchment variables produced in the above scripts
- **streamresponseBayesModel** runs Bayesian generalized mixed-effects models to evaluate MI60, fire, year, snow zone, NDVI, and catchment variables effect on stream response
