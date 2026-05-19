# Interim Report Drafting Outline

## Working Title

Explainable Machine Learning for Wind-Turbine Maintenance Triage Using Public Supervisory Control and Data Acquisition Data

## Current Methodological Status

The project has completed the data acquisition, decompression, raw audit, Parquet conversion, duplicate timestamp resolution, timestamp-gap audit, chronological split, strict label-source discovery, proxy-label construction, and visual exploratory data analysis stages.

The current labels are proxy operational labels produced from train-fitted power-curve behaviour. They are useful for interim analysis but should not be described as verified alarm-event labels.

## Recommended Tables

1. Table 1. Data Processing Summary.
2. Table 2. Chronological Split Summary.
3. Table 3. Feature-Screening Summary.
4. Table 4. Proxy Label Distribution.
5. Table 5. Timestamp Gap Summary.
6. Table 6. Preliminary Model Metrics.

## Recommended Figures

1. Figure 1. Training Split Proxy Label Distribution.
2. Figure 2. Proxy Label Mix by Turbine.
3. Figure 3. Training Split Power Curve by Proxy Label.
4. Figure 4. Median Power Curve by Turbine.
5. Figure 5. Timestamp Coverage Ratio by Turbine.
6. Figure 6. Timestamp Gap Duration Distribution.
7. Figure 7. Preliminary Model Macro-F1 Comparison.
8. Figure 8. Preliminary Random Forest Feature Importance.

## Report Positioning

The interim report should present the current modelling results as preliminary proxy-supervised results. The final capstone should continue searching for true time-stamped alarm-event labels or incorporate an external labelled benchmark such as CARE.