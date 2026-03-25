# Ventral Subiculum Neuron Spatial Analysis

This project explores the spatial distribution of neurons in the ventral subiculum (vS) projecting to different brain regions:
- PFC (prefrontal cortex)
- NAc (nucleus accumbens)
- LH (lateral hypothalamus)

Using anatomical coordinates (AP, ML, DV), we visualise and compare how neuron populations differ in space.

## Dataset

Data from:
Wee & MacAskill (2020)  
"Biased Connectivity of Brain-wide Inputs to Ventral Subiculum Output Neurons" at https://www.sciencedirect.com/science/article/pii/S2211124720302679?ref=pdf_download&fr=RR-2&rr=9e1f7a006838417f

Each dataset contains neuron coordinates:
- **AP (Anterior–Posterior)**
- **ML (Medial–Lateral)**
- **DV (Dorsal–Ventral)**

Three datasets were combined into a single dataframe for analysis.

## Analysis Overview

### 1. 3D Spatial Visualisation

Interactive 3D scatter plot showing neuron positions across AP, ML, DV axes.

- Colour indicates projection target (PFC, NAc, LH)
- Reveals overall structure and overlap between populations
![3D Plot](projection_3d.png)

### 2. Cumulative Distribution (ECDF)

Cumulative distribution plots along each axis:
- AP
- ML
- DV
![ECDF Plot](ecdf_subplots.png)

**Interpretation:**
At a given coordinate value, the ECDF shows the fraction of neurons located at or below that point.

This allows comparison of spatial bias between projection targets.

### 3. Box Plots

Distribution of neuron positions along each axis grouped by projection target.

- Highlights median differences
- Shows spread and outliers
- Enables clear comparison across PFC, NAc, LH
![Box Plot](boxplot_distribution.png)

### 4. Summary Statistics

Mean spatial coordinates were computed for each projection target to quantify differences.

## Key Insights

- Neurons projecting to different targets show **subtle but consistent spatial biases**
- i.e. Overlapping but not distinct
- Differences are most visible in:
  - AP (anterior–posterior)
  - DV (depth)
- ML axis shows more gradual variation
