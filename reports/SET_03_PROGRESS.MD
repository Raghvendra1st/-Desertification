
# Progress Report – Set 3: System Design & Logic
**Project:** AI for Prediction  Desertification Patterns  
**Group ID:** 101  
**Date:** March 14, 2026

## 1. Overview
During this phase, the project transitioned from theoretical research to the **Architectural Design** stage. We focused on defining how data flows through our system and selecting the specific technologies required for implementation.

## 2. Work Accomplished
The following milestones were achieved during this reporting period:

### A. System Architecture Design
We designed a high-level architecture that connects our data sources to our predictive model.
* **Data Ingestion:** Using cloud-based APIs to fetch satellite imagery.
* **Pre-processing Layer:** Scripts to remove noise (clouds/shadows) and calculate vegetation health.
* **Learning Core:** A Neural Network structure designed to recognize patterns over time.

### B. Data Flow Diagram (DFD)
We mapped the movement of information within the project:
1.  **Input:** Multi-spectral imagery (Visible and Infrared light) from satellites.
2.  **Transformation:** Converting raw pixels into readable indices (like NDVI).
3.  **Storage:** Staging processed data for the AI to "read."
4.  **Output:** A visual map showing predicted desert expansion zones.

### C. Technology Stack Selection
To ensure project stability, we finalized the following tools:
* **Google Earth Engine (GEE):** For accessing massive satellite datasets without heavy local downloads.
* **Python:** The primary programming language for data manipulation.
* **TensorFlow/Keras:** The framework used to build and train the AI model.
* **QGIS:** For final map visualization and geographical verification.

## 3. Technical Justification (The "Why")
* **Why Sentinel-2?** It provides high-resolution (10m) data, allowing us to see small changes in land quality.
* **Why AI?** Traditional methods only show *current* desertification; our AI approach identifies *patterns* to predict where the desert will move next.

## 4. Work Planned for Next Period
* Begin active data collection for the selected study area.
* Develop the "Cloud Masking" script to clean incoming satellite images.
* Perform initial Exploratory Data Analysis (EDA) to verify data quality.

