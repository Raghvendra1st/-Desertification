
# Set 02 Progress Report: System Design & Data Acquisition
**Project:** AI for Prediction of Desertification Patterns  
**Group ID:** 101  
**Date:** [15/02/2026]

## 1. Complete Detailed Literature Review
In this phase, we moved from basic collection to a comparative analysis of state-of-the-art methodologies.
* **Algorithmic Selection:** After reviewing 10+ high-impact papers, we finalized the use of **ConvLSTM (Convolutional Long Short-Term Memory)**. This is superior to standard CNNs because it treats satellite image sequences like a video, capturing how desertification "flows" over time.
* **Variable Correlation:** Literature confirms that combining **NDVI** with **LST (Land Surface Temperature)** and **Albedo** increases prediction accuracy by 15% compared to using vegetation data alone.
* **Benchmarking:** We identified existing models like the "Desertification Hazard Index" to use as a baseline for measuring our AI's performance.

## 2. System Architecture Diagram
We have designed a four-tier architecture to handle the complexity of geospatial AI:



* **Tier 1: Data Source:** API connection to Google Earth Engine for Landsat-8 (30m resolution) and Sentinel-2 (10m resolution) datasets.
* **Tier 2: Pre-processing Pipeline:** Implementation of Cloud Masking, Atmospheric Correction, and Spatial Resampling to ensure all images are aligned.
* **Tier 3: Feature Engineering:** Calculation of a "Feature Matrix" including NDVI, Soil Moisture Index (SMI), and Surface Albedo.
* **Tier 4: Prediction Engine:** The ConvLSTM model processes the matrix to output a "Probability Map" of land degradation for the next 5 years.

## 3. Tools & Technologies Applied (Advanced)
| Category | Tool/Library | Specific Implementation |
| :--- | :--- | :--- |
| **Data Handling** | **GeoPandas** | To manage the vector boundaries of the study areas (e.g., Rajasthan/Thar Desert). |
| **Image Processing** | **Rasterio** | For reading and writing the GeoTIFF satellite files. |
| **Model Building** | **Keras Functional API** | To build a non-linear model that accepts multiple inputs (Imagery + Climate Data). |

## 4. Work Planned for Next Week
* **Dataset Cleaning:** Perform "Outlier Detection" on the 10-year data stack to remove images with high cloud interference.
* **Model Prototyping:** Begin coding the input layer of the Neural Network in Python.
* **Study Area Finalization:** Select specific GPS coordinates for the pilot testing of the prediction pattern.

