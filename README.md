# Using PCA to identify process anomalies

In this study, the algorithm of Principal Component Analysis was applied to detect and identify anomalies in process data.
This application shows an opportunity to integrate process analysis and machine learning techniques.

## Introduction

The main motivation of detection and identification of process anomalies is quality control. Quality problems occur due to process variations and generate waste of resources. When working with process improvement, the root causes of quality deviations should be identified and properly treated.

The PCA approach presents an opportunity to improve the identification of anomalies, because it permits to detect potential problems based on multivariate statistical concepts. 

## Methodology

The presented study has the following approach and steps:

### Process Simulation

First step was to simulate a simple process and to define the measured variables. The process chosen for this study was a simple unit operation of mixing, and the observed variables were:
- inlet mass flow rates of three components;
- inlet concentrations of two components
- outlet concentrations of two components

The process was simulated for 70,000 data points, to explore different operating conditions and to determine the sources of process variations.

### Variable Correlation Study

After obtaining the process data point, an exploratory data analysis was conducted to understand the correlations between process variables, and to determine which ones are the most critical to process variations.

### PCA Training

The dataset was treated and filtered to select only the "normal operation data". This subset was submitted to PCA training.

### Anomaly Detection and Identification

Based on PCA results, the data points were classified as "normal" or "anomaly". The classification was based on hypothesis test.
When a point was classified as "anomaly", the algorithm was set to explore such point and to determine which sensor promoteof d the major contribution.
Also is was to possible to visualize the contribution plots of each anomaly detected.
